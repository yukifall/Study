 protected override IKernel CreateKernel()
{
    var kernel = new StandardKernel();
    kernel.Load(Assembly.GetExecutingAssembly());
    kernel.Bind<IRenderHelper>().To<RenderHelper>();

    GlobalConfiguration.Configuration.ServiceResolver.SetResolver(new NinjectDependencyResolver(kernel));
    return kernel;
}
