
// QUESTION FIVE (a)
// DECLARING VARIABLES

let studentName = "John";
let registrationNumber = "COM/B/01-001/2025";
let programme = "Computer Science";

console.log(studentName);
console.log(registrationNumber);
console.log(programme);


// QUESTION FIVE (b)
// FUNCTION TO CALCULATE GRADE

function calculateGrade(score) {

    if (score >= 70) {
        return "A";
    }
    else if (score >= 60) {
        return "B";
    }
    else if (score >= 50) {
        return "C";
    }
    else if (score >= 40) {
        return "D";
    }
    else {
        return "E";
    }
}


// QUESTION FIVE (c)
// CALL FUNCTION

let grade = calculateGrade(75);
alert("Your grade is: " + grade);


// QUESTION SIX AND SEVEN
// DOM MANIPULATION AND FORM VALIDATION

let form = document.getElementById("registrationForm");

form.addEventListener("submit", function(event) {

    // PREVENT DEFAULT SUBMISSION
    event.preventDefault();

    // RETRIEVE STUDENT DETAILS
    let name = document.getElementById("name").value.trim();
    let regNo = document.getElementById("regNo").value.trim();
    let email = document.getElementById("email").value.trim();

    // VALIDATE NAME AND REGISTRATION NUMBER
    if (name === "" || regNo === "") {
        alert("Please fill in your name and registration number.");
        return;
    }

    // VALIDATE EMAIL
    let emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;

    if (!emailPattern.test(email)) {
        alert("Please enter a valid email address.");
        return;
    }

    // DISPLAY STUDENT DETAILS
    document.getElementById("result").innerHTML =
        "<h3>Registration Successful!</h3>" +
        "<p>Student Name: " + name + "</p>" +
        "<p>Registration Number: " + regNo + "</p>" +
        "<p>Success! Your details have been submitted.</p>";

    alert("Registration Successful!");

});
