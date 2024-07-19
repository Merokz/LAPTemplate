App works best with [EFCorePowerTools](https://marketplace.visualstudio.com/items?itemName=ErikEJ.EFCorePowerTools)

## Change the Connectionstring in _Appsettings.json_:
replace: <code>Data Source=(localdb)\\MSSQLLocalDB;Initial Catalog=EXAMPLE; <code/>  

## Update your **DBContext** in _Program.cs_
<code>//builder.Services.AddDbContext<LapTestContext>(options =>
//{
//    options.UseSqlServer(builder.Configuration.GetConnectionString("DefaultConnection"));
//});</code>

replace => **LapTestContext** with your actual __DBContext__

This Template is based on the MS-MVC Project Template.
