
# Team-Profile-Generator
* This application is a team generator command line application.

* I used the [Inquirer npm package](https://github.com/SBoudrias/Inquirer.js/) to prompt the * user for their email, id, and specific information based on their role with the company.

 * In addition to this set of information intern must also provide their school, engineers must provide their GitHub username and managers must provide their office number.

* The app will run as a Node CLI to gather information about each employee.


 # installation

* In the `Develop` folder, there is a `package.json`, so to use this file you must sure to `npm install` in the command line.

* The dependencies are, [jest](https://jestjs.io/) for running the provided tests, and [inquirer](https://www.npmjs.com/package/inquirer) for collecting input from the user.



## Classes

The project has classes: `Employee`, `Manager`, `Engineer`,
`Intern`. 

The first class is an `Employee` parent class with the following properties and
methods:
```
  * name
  * id
  * email
  * getName()
  * getId()
  * getEmail()
  * getRole() // Returns 'Employee'
```

The other three classes extend `Employee`. 

In addition to `Employee`'s properties and methods, `Manager` has:
```
  * officeNumber
  
  * getOfficeNumber()

  * getRole() // Overridden to return 'Manager'
```
In addition to `Employee`'s properties and methods, `Engineer` has:
```
  * github  // GitHub username

  * getGithub()

  * getRole() // Overridden to return 'Engineer'
```
In addition to `Employee`'s properties and methods, `Intern` has:
```
  * school 

  * getSchool()

  * getRole() // Overridden to return 'Intern'
```

The project generates a `team.html` page in the `output` directory, that displays a nicely formatted team roster. Each team member displays the following:
```
  * Name

  * Role

  * ID

  * Role-specific property (School, link to GitHub profile, or office number)
```

 All unit tests are passing.
