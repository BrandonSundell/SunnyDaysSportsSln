# SunnyDaysSportsSln
In class exercise where we create a Sports store application so a user can buy products using sample code from our text book and the instructor. THIS IS A MSSA IN CLASS PROJECT FOR DEMINSTRATION PURPOSES ONLY! 

## Link To Book
"https://www.apress.com/gp/book/9781484254394"

## Build Script

      dotnet new globaljson --sdk-version 5.0.104 --output SunnyDaysSportsSln/SunnyDaysSports
      dotnet new web --no-https --output SunnyDaysSportsSln/SunnyDaysSports --framework net5.0
      dotnet new sln -o SunnyDaysSportsSln
      dotnet sln SunnyDaysSportsSln add SunnyDaysSportsSln/SunnyDaysSports
      dotnet new xunit -o SunnyDaysSportsSln/SunnyDaysSports.Tests --framework net5.0
      dotnet sln SunnyDaysSportsSln add SunnyDaysSportsSln/SunnyDaysSports.Tests 
      dotnet add SunnyDaysSportsSln/SunnyDaysSports.Tests reference SunnyDaysSportsSln/SunnyDaysSports
