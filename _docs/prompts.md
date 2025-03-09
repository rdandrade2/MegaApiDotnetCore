contexto:
Este projeto é um projeto de uma api feito em dotnet, para listar os dados dos bosses de megaman, o objetivo principal é ser um backend que fornece jsons no formato abaixo:

"""
{ 
                        Id =1,
                        Code = "DLN/DRN-003",
                        Name = "Cutman",
                        HP = 150,
                        Picture = "https://vignette.wikia.nocookie.net/megaman/images/2/22/Cutman.png"
                }

"""

Especificações do projeto:
"""
<Project Sdk="Microsoft.NET.Sdk.Web">

  <PropertyGroup>
    <TargetFramework>netcoreapp3.1</TargetFramework>
  </PropertyGroup>

  <ItemGroup>
    <PackageReference Include="Microsoft.EntityFrameworkCore" Version="3.1.8" />
    <PackageReference Include="Microsoft.EntityFrameworkCore.Design" Version="3.1.8">
      <IncludeAssets>runtime; build; native; contentfiles; analyzers; buildtransitive</IncludeAssets>
      <PrivateAssets>all</PrivateAssets>
    </PackageReference>
    <PackageReference Include="Microsoft.EntityFrameworkCore.SqlServer" Version="3.1.8" />
    <PackageReference Include="Newtonsoft.Json" Version="12.0.2" />
  </ItemGroup>

</Project>
"""

REGRAS:
-Sempre que citar alguma dependência do projeto, deixe ela como hyperlink para página oficial daquela dependência 




na parte de estrutura do projeto insira este mapeamento de pastas:./src
./src/.vs
./src/.vs/MegamanApi
./src/.vs/MegamanApi/v15
./src/.vscode
./src/bin
./src/bin/Debug
./src/bin/Debug/netcoreapp3.1
./src/bin/Debug/netcoreapp3.1/Properties
./src/bin/Debug/netcoreapp3.1/runtimes
./src/bin/Debug/netcoreapp3.1/runtimes/unix
./src/bin/Debug/netcoreapp3.1/runtimes/unix/lib
./src/bin/Debug/netcoreapp3.1/runtimes/unix/lib/netcoreapp2.0
./src/bin/Debug/netcoreapp3.1/runtimes/unix/lib/netcoreapp2.1
./src/bin/Debug/netcoreapp3.1/runtimes/win
./src/bin/Debug/netcoreapp3.1/runtimes/win/lib
./src/bin/Debug/netcoreapp3.1/runtimes/win/lib/netcoreapp2.0
./src/bin/Debug/netcoreapp3.1/runtimes/win/lib/netcoreapp2.1
./src/bin/Debug/netcoreapp3.1/runtimes/win/lib/netstandard2.0
./src/bin/Debug/netcoreapp3.1/runtimes/win-arm64
./src/bin/Debug/netcoreapp3.1/runtimes/win-arm64/native
./src/bin/Debug/netcoreapp3.1/runtimes/win-x64
./src/bin/Debug/netcoreapp3.1/runtimes/win-x64/native
./src/bin/Debug/netcoreapp3.1/runtimes/win-x86
./src/bin/Debug/netcoreapp3.1/runtimes/win-x86/native
./src/Controllers
./src/Database
./src/Database/DTOs
./src/Database/DTOs/Robots
./src/Database/EntityFramework
./src/Database/EntityFramework/Context
./src/Database/EntityFramework/Migrations
./src/Database/Repositories
./src/Database/Repositories/Robots
./src/middlewares
./src/Models
./src/obj
./src/obj/Debug
./src/obj/Debug/netcoreapp3.1
./src/obj/Debug/netcoreapp3.1/staticwebassets
./src/Properties
./src/Services
./src/Services/Robots
./_docs
./_docs/assets