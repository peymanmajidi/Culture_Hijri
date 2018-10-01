# Culture_Hijri
Hijri Culture Intialize all C# Projects

This is a wondeful library you can simply add to your c# projects.
It works like magic ! Convert every use of DateTime to Persion Culture
Even SQL Server Transactions

Persian Hint: تبدیل کلیه تاریخ ها به هجری شمسی


## ASP.Net MVC Projects
Solution Explorer > Global.asax.cs

        protected void Application_Start()
        {
            AreaRegistration.RegisterAllAreas();
            FilterConfig.RegisterGlobalFilters(GlobalFilters.Filters);
            RouteConfig.RegisterRoutes(RouteTable.Routes);

            BundleConfig.RegisterBundles(BundleTable.Bundles);
            Cultures.InitializePersianCulture(); // <-------------------------- add this line

        }

## C# Projects

Solution Explorer > Program.cs

     private static void Main()
        {
            Cultures.InitializePersianCulture(); // <--------------------------
        }	


