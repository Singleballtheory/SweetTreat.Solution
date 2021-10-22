# Pierre's Sweat and Savory Treats

#### The sweet-tooth oasis with the unfortunate name

#### By Scott Hutley

## Technologies Used

* _C#_
* _.Net 5.0_
* _.Net ef_
* _ASP.NET Core_
* _NuGet_

## Description

Pierre's ever-expanding empire of eateries has entered into the realm of diabetes-inducing confections. Unfortunately for him, he went cheap on the signage so all his logos and merchandise suggest something less enticing are in his treats. When I told him we could still create the website with the proper name, Pierre chose instead to double-down on the name change by declaring "All my blood, _sweat_ and tears has gone into this place! Leave it!" Zut alors, Pierre!

## Setup/Installation

#### Technology Requirements

* .NET 5
* VS Code or other text editor
* MySQL Workbench

#### Cloning and Database Creation

* Clone this repository to your desktop
* Open with text editor and navigate into SweetTreat.Solution/SweetTreat folder
* Create an appsettings.json file
* Add the following code to the appsettings.json:
```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=sweet_treat;uid=root;pwd=YOUR_PASSWORD;"
  }
}
```
* Replace "YOUR_PASSWORD" in the above code with your own personal MySql password
* Open a Windows Powershell terminal (or Mac equivalent)
* In that terminal run *mysql -uroot -p<YOUR_PASSWORD>* (again, replacing with your actual password)
* Open MySQL Workbench
* Return to your text editor
* Navigate to the SweetTreat.Solution/SweetTreat folder level (if you are not already there)
* Run *dotnet restore*
* Run *dotnet build*
* Run *dotnet run* to use the app!
(note: If dotnet run does not auto-generate a browser page, you can manually enter http://localhost:5000 into your web browser)

## Known Bugs

* Currently "Flavors" can be added by all users, even ones who are not logged in. This is intended to be a feature for users to let Pierre know what flavors they might be interested in, but people keep adding really horrible flavors to the list or simply editing the ones that already exist into some really nasty stuff. As such, restrictions will likely need to be put in place.

## License

_[MIT](https://opensource.org/licenses/MIT)_

Copywrite(c)2021 Scott Hutley

## Contact Information

Scott Hutley: scotthutley1@comcast.net