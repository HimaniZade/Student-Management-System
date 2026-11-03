const form = document.getElementById("studentForm");
const studentList = document.getElementById("studentList");

form.addEventListener("submit", function(event) {
    event.preventDefault();

    const name = document.getElementById("name").value.trim();
    const roll = document.getElementById("roll").value.trim();
    const course = document.getElementById("course").value.trim();

    const row = document.createElement("tr");

    [name, roll, course].forEach(function(value) {
        const cell = document.createElement("td");
        cell.textContent = value;
        row.appendChild(cell);
    });

    const actionCell = document.createElement("td");
    const deleteButton = document.createElement("button");

    deleteButton.type = "button";
    deleteButton.textContent = "Delete";

    deleteButton.addEventListener("click", function() {
        row.remove();
    });

    actionCell.appendChild(deleteButton);
    row.appendChild(actionCell);

    studentList.appendChild(row);

    form.reset();
});
