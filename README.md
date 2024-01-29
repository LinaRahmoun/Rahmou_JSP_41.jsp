# Rahmou_JSP_41.jsp
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>Rahmoun JSP 41</title>
    <style>
        table {
            border-collapse: collapse;
            width: 50%;
            margin: 20px;
        }
        th, td {
            border: 1px solid black;
            padding: 8px;
            text-align: left;
        }
    </style>
</head>
<body>
    <%
        int[] intArray = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
        String[] stringArray = {"Apple", "Banana", "Orange", "Grapes", "Mango"};
    %>

    <h2>Integer Array</h2>
    <table>
        <tr>
            <th>Index</th>
            <th>Element</th>
            <th>Type</th>
        </tr>
        <%
            for (int i = 0; i < intArray.length; i++) {
        %>
                <tr>
                    <td><%= i %></td>
                    <td><%= intArray[i] %></td>
                    <td><%= (intArray[i] % 2 == 0) ? "Even" : "Odd" %></td>
                </tr>
        <%
            }
        %>
    </table>

    <h2>String Array</h2>
    <table>
        <tr>
            <th>Index</th>
            <th>Element</th>
        </tr>
        <%
            for (int i = 0; i < stringArray.length; i++) {
        %>
                <tr>
                    <td><%= i %></td>
                    <td><%= stringArray[i] %></td>
                </tr>
        <%
            }
        %>
    </table>
</body>
</html>
