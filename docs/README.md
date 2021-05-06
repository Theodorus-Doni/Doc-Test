<br>
<p align="center">
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://lncodes.com">
    <img src="https://lncodes.com/wp-content/uploads/2020/09/lncodes-logo-animated.gif" height="175"></img>
  </a>
</p>

<h1 align="center">EXPORT IMPORT CSV PACKAGE ( VLECIS )</h1>

<p align="center">
  <a href="https://github.com/lncodes/vlecis/actions/workflows/build.yml">
    <img src="https://github.com/lncodes/vlecis/actions/workflows/build.yml/badge.svg">
  </a> 
  <a href="https://github.com/lncodes/vlecis/actions/workflows/test.yml">
    <img src="https://github.com/lncodes/vlecis/actions/workflows/test.yml/badge.svg">
  </a>
  <a href="https://sonarcloud.io/dashboard?id=lncodes_vlecis">
    <img src="https://sonarcloud.io/api/project_badges/measure?project=lncodes_vlecis&metric=alert_status">
  </a>
</p>

<p align="center">
  <a href="#introduction">Introduction</a> •
  <a href="#setup">Setup</a> •
  <a href="#contribute">Contribute</a> •
  <a href="#discuss">Discuss</a> •
  <a href="#support">Support</a> •
  <a href="#license">License</a>
</p>

---

<h2 id="introduction">✨ Introduction</h2>

Vlecis is package that used to export and import CSV package, for more information about this project, you can refer to [Documentation](https://lncodes.com/studio/package/csharp-export-import-csv/).

<h3 id="scope">🎯 Scope</h3>
The main objective of the project is { *Objective of the project* }

<h2 id="setup">🧰 Setup </h2>

### 🔧 Requirements
- Installed .NET 3.1 SDK
- 
### ⚙️ Installation 
Follow these steps to install **VLECIS**
1. Clone/Download the *vlecis* package.
``` bash 
git clone https://github.com/lncodes/vlecis.git
```
2. Open and build the *vlecis* package.

<img src="media/add-vlecis-dependency.gif" height="240"/>

3. Add package depedency to your project.

<img src="media/add-vlecis-dependency.gif" height="240"/>

> You can use NuGet to add VLECIS package to your project.

### 💻 Usage
Follow these steps to use **VLECIS** package.
1. Import vlecis package and fathgen module namespace to your class.
``` c#
using Lncodes.Pacakge.Vlecis;

namespace Lncodes.Vlecis.Result
{
    public class Program
    {
        
    }
}

```
2. Make vlecis class instance with class that you want to import.
``` c#
using Lncodes.Pacakge.Vlecis;
using Lncodes.Module.Fathgen;

namespace Lncodes.Vlecis.Result
{
    public class Program
    {
        private static void main(string[] args) 
        {
            var filePathGenerator = new FilePathGenerator<CsvFileExtension>("FileName", CsvFileExtension.CSV);
            var config = new VlecisConfig(filePathGenerator);
            var vlecis = new Vlecis<MockData>(config);
        }
    }
}
```
3. Call export/import method.
``` c#
using Lncodes.Pacakge.Vlecis;

namespace Lncodes.Vlecis.Result
{
    public class Program
    {
        private static void main(string[] args) 
        {
            var filePathGenerator = new FilePathGenerator<CsvFileExtension>("FileName", CsvFileExtension.CSV);
            var config = new VlecisConfig();
            var vlecis = new Vlecis<MockData>(config);

            var mockData = new MockData();
            vlecis.ExportFrom(mockDataWithValue);
            vlecis.ImportTo(mockData);
        }
    }
}
```
> For more information you can visit the [Documentation](https://lncodes.com/studio/package/csharp-export-import-csv/) page.

<h2 id="contribute">💖 Contribute</h2>

Want to contribute to this project? Please read our project [Contribution Guidelines](CONTRIBUTING.md).

<h2 id="discuss">💬 Discuss</h2>

If you have any questions about this project, you can go to [Discussion Forum](https://github.com/lncodes/vlecis/discussions) or directly comment on [Documentation](https://lncodes.com/studio/package/csharp-export-import-csv/) page.

<h2 id="support">💌 Support</h2>

Please support us to make other helpful content.

<a href="https://www.buymeacoffee.com/lncodes" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" height="64"></a>

<h2 id="license">	📋 License</h2>

This project is open-sourced software licensed under [MIT](https://github.com/lncodes/vlecis/blob/master/LICENSE) license.
