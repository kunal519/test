# test
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        .accordion {
            display: flex;
            flex-direction: column;
            width: 300px;
            margin: 20px;
        }

        .accordion input {
            display: none;
        }

        .accordion label {
            background-color: #ddd;
            padding: 10px;
            cursor: pointer;
            user-select: none;
        }

        .accordion-content {
            display: none;
            padding: 10px;
            border-top: 1px solid #ccc;
        }

        .accordion input:checked + label + .accordion-content {
            display: block;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }

        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
    </style>
</head>
<body>

    <div class="accordion">
        <input type="checkbox" id="section1">
        <label for="section1">Section 1</label>
        <div class="accordion-content">
            <table>
                <tr>
                    <th>Header 1</th>
                    <th>Header 2</th>
                </tr>
                <tr>
                    <td>Data 1</td>
                    <td>Data 2</td>
                </tr>
            </table>
        </div>
    </div>

    <div class="accordion">
        <input type="checkbox" id="section2">
        <label for="section2">Section 2</label>
        <div class="accordion-content">
            <table>
                <tr>
                    <th>Header A</th>
                    <th>Header B</th>
                </tr>
                <tr>
                    <td>Data A</td>
                    <td>Data B</td>
                </tr>
            </table>
        </div>
    </div>

</body>
</html>
