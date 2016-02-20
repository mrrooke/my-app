---
layout: post
title: Y11 Checklist
list: true
---
The table below contains all the topics that you will need to understand for your exam in the summer. You can either look at the table below (clicking on the first row will sort), or click [here][56253a7d] to download an excel file that you can print.

<table id="data">
    <thead>
    </thead>
    <tbody>
    </tbody>
</table>
<script src="d3js.org/d3.v3.min.js">
    d3.csv('y11SOW.csv', function(error, data) {
        if (error) throw error;
        var columns = ['Area', 'Topic', 'Grade', 'Covered']
        tabulate(data, columns);
    });

    function tabulate(data, columns) {
        var table = d3.select("table"),
            thead = table.select("thead"),
            tbody = table.select("tbody");

        thead.selectAll("th")
            .data(columns)
            .enter()
            .append("th")
            .text(function(column) {
                return column;
            });

        var previousSort = null
        d3.selectAll("thead th").data(columns).on("click", function(k) {
            if(k != previousSort) {
                    rows.sort(
                        function(a,b) {
                            return d3.ascending(a[k],b[k]);
                        }
                    )

            previousSort = k;}
            else{
                rows.sort(
                    function(a,b) {
                        return d3.descending(a[k],b[k]);
                    }
                )
                previousSort = null;
            }

        })

        // create a row for each object in the data
        var rows = tbody.selectAll("tr")
            .data(data)
            .enter()
            .append("tr");

        // create a cell in each row for each column
        var cells = rows.selectAll("td")
            .data(function(row) {
                return columns.map(function(column) {
                    return {
                        column: column,
                        value: row[column]
                    };
                });
            })
            .enter()
            .append("td")
            .text(function(d) {
                return d.value;
            });
    }
</script>

 [56253a7d]: /resources/checklist.xlsx "here"
