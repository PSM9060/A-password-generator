# A-password-generator
let length = parseInt(prompt("Enter password length:"));

let characters = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#$%^&*()";
let password = "";

for (let i = 0; i < length; i++) {
  let randomIndex = Math.floor(Math.random() * characters.length);
  password += characters[randomIndex];
}

alert("Your generated password is:\n" + password);
