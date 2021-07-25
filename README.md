# Assignment
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hamza</title>
</head>

<body>
    <form action="app.js"></form>
    <label for="Name"><h4>Name</h4></label>
    <input type="text" name="Name" id="Name">

    <label for="Gender" id="Gender"> <h4>Gender</h4></label>
    <label for="Male">Male</label>
    <input type="radio" name="Gender" value="Male" id="Male">
    <label for="female">Female</label>
    <input type="radio" name="Gender" value="Female" id="female">

    <label for="Address"><h4>Address</h4></label><br>
    <textarea name="Address" id="Address" cols="30" rows="10">Address</textarea>

    <label for="Educaton" id="Education"><h4>Education</h4></label><br>
    <label for="Matric" >Matric</label>
    <input type="radio" name="Education" value="Matric" id="Matric">
    <label for="Inter">Inter</label>
    <input type="radio" name="Education" value="Inter" id="Inter">
    <label for="graduate">Graduate</label>
    <input type="radio" name="Education" value="graduate" id="graduate">

    <label for="Profession" id="Profession"><h4>Profession</h4></label>
    <select name="Profession" id="Profession">
        <option value="Engineer">Engineer</option>
        <option value="Doctor">Doctor</option>
        <option value="Chef">Chef</option>
        <option value="Self Empolyeed">Self Empolyeed</option>
      </select> <br>

    <button type="submit"><H3>Submit</H3></button>

    <script >// Question 1
var itemsArray = [
{name:"juice",price:"50", quantity:"3"},
{name:"cookie",price:"30", quantity:"9"},
{name:"shirt",price:"880", quantity:"1"},
{name:"pen",price:"100", quantity:"2"}];
var priceOFJuice = itemsArray[0].price * itemsArray[0].quantity
var priceOFCookie = itemsArray[1].price * itemsArray[1].quantity
var priceOfShirt = itemsArray[2].price * itemsArray[2].quantity
var priceOfPen = itemsArray[3].price * itemsArray[3].quantity
var totalPriceOFAll = priceOFCookie + priceOFJuice + priceOfPen + priceOfShirt

console.log( "Shirt = " +  priceOfShirt , ", Cookie = " + priceOFCookie, ", pen = " +  priceOfPen, ", Juice = " + priceOFJuice)
console.log( "Total Price of All Itmes is " +  totalPriceOFAll)



//Question 2
var obj = {
    name:"Hamza",
    email:"sample@gmail.com",
    Password:123456,
    age :"21",
    Gender:"male",
    City:"Karachi",
    Country:"Pakistan",
}
var check = obj.City;
var check2 = obj.age;

console.log(check, check2)

//Question 3
function User(Name, age , Hobby , fvrtColor){
    this.fullname=Name,
    this,umar= age,
    this,mashgala= Hobby,
    this.color= fvrtColor
}

var user1 = new User("Hamza", 21, "Football", "orange");
var user2 = new User("Faiz" , 15, "Cricket", "Green");
var user3 = new User("Owais", 20, "Anime", "yellow" );

console.log(user1, user2, user3);

// Question 4
function User(Name, Gender, Address, Education, Profession){
    this.Name=Name,
    this.Address=Address,   
    this.Gender=Gender,     
    this.Education=Education
    this.Profession=Profession
}
var userName = document.getElementById("Name");
var userGender= document.getElementById("Gender");
var userAddress= document.getElementById("Address");
var userEducation= document.getElementById("Education");
var userProfession=document.getElementById("Profession");
var arr = [ ]
var myuser1 = new User(userName.value, userGender.value, userEducation.value, userAddress.value, userProfession.value );
arr.push(myuser1)
console.log(myuser1);
</script>
</body>

</html>
