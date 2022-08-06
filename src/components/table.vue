<template>
<div class="header">
        <h1>
            College degrees earned to date and those you currently working towards
        </h1>
    </div>
</template>

<script>
 new Vue({
    el:'#app',
    data: {
        columns: [
          'School',
          'Program',
          'Type',
          'Graduation_Date'  
        ]
    }
 })

 document.addEventListener("DOMContentLoaded", function(event){
    fetch("https://ptsv2.com/t/jordan/post")
    .then((res) => res.json())
    .then((data) => {
        console.log("The fetched data: ", data);

        const table = document.createElement("table");

        let tr = document.createElement("tr");

        addHead(tr, "School");
        addHead(tr, "Program");
        addHead(tr, "Type");
        addHead(tr, "Graduation_Date");

    table.appendChild(tr);

        let td1 = '';
        let td2 = '';
        let td3 = '';
        let td4 = '';

    data.Degrees.forEach((element, index) => {
        console.log("Raw data ", element);

        tr = document.createElement("tr");
        td1 = document.createElement("td");
        td2 = document.createElement("td");
        td3 = document.createElement("td");
        td4 = document.createElement("td");

        content = document.createTextNode(element.School);
        td1.appendChild(content);
        content = document.createTextNode(element.Program);
        td2.appendChild(content);
        content = document.createTextNode(element.Type);
        td3.appendChild(content);
        content = document.createTextNode(element.Graduation_Date);
        td4.appendChild(content);

        tr.appendChild(td1);
        tr.appendChild(td2);
        tr.appendChild(td3);
        tr.appendChild(td4);

        table.appendChild(tr);
    });
    document.body.appendChild(table);
    });
});

function addHead(row, headTitle) {
    head = document.createElement("th");
    txt = document.createTextNode(headTitle);
    head.appendChild(txt);
    row.appendChild(head);
}

</script>


<style>
  .header {
    display: flex;
    justify-content: center;
    border: #dddddd;
    background-color: aqua;
    text-align: center;
  }
  table {
    font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    border-collapse: collapse;
    width: 100%;
    height: 12vh;
    font-size: large;
  }
  
  td, th {
    border: 1px solid #dddddd;
    text-align: left;
    padding: 5px;
  }
  
  tr:nth-child(even) {
    background-color: #dddddd;
  }

</style>