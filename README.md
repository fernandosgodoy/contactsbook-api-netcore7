# Contacts Book - .NET Core 7 API Project demo
This is a demo API, developed in .NET Core 7, using the Microsoft SQL Server database and hosted in a Docker container.
The scenario or problem chosen was a simple contact list, which will serve a front-end application in any future stack chosen.
Below I demonstrate some steps to execute the application and if you have any questions, we will talk to you during the technical interview.


## Database diagram
![image](https://github.com/fernandosgodoy/contactsbook-api-netcore7/assets/1747058/24745975-61d8-4649-a655-13a06fee6912)

## Run Docker image
To run the Docker image, open the PowerShell (or another command line app) and run the command:

`
dotnet publish --os linux --arch x64 -p:PublishProfile=DefaultContainer -c Release
`

Running the command on Visual Studio console window (PowerShell):
![image](https://github.com/fernandosgodoy/contactsbook-api-netcore7/assets/1747058/f9b5f429-e455-4dc7-9789-a421f6634638)

This command will create the image and you can run you instance:
![image](https://github.com/fernandosgodoy/contactsbook-api-netcore7/assets/1747058/30d44572-072f-4413-aae3-9f580467fea4)

Instead of create an image, you can run the Docker Compose command and use the attached file docker-compose.yml inside the ContactBookApi project

## Unit tests
All the development was done using the TDD approach and this is the manner that I really believe who is good to detect problems, refactory code and maintain the App. All the tests were developed using th XUnit library, and you'll see in the project like this:
![image](https://github.com/fernandosgodoy/contactsbook-api-netcore7/assets/1747058/af734a56-680c-45fb-af74-10be01308ad8)


