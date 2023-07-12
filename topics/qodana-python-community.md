[//]: # (title: Qodana Community for Python)

[![official project](https://jb.gg/badges/official-flat-square.svg)](https://confluence.jetbrains.com/display/ALL/JetBrains+on+GitHub)

<img src="python.png" dark-src="python_dark.png" alt="Python" width="296"/>

<note>
    <p>
<include src="lib_qd.xml" include-id="eap-warning">
<var name="product" value="Qodana Community Python"/>
</include>
</p>
</note>

<var name="linter" value="Qodana Community Python"/>
<var name="ide" value="PyCharm Community"/>
<var name="docker-image" value="jetbrains/qodana-python-community:2023.2-eap"/>

%linter% is based on [%ide%](https://www.jetbrains.com/pycharm/) and provides static analysis for Python projects.

%linter% provides inspections for the following technologies.

<table header-style="none">
    <tr>
        <td>Programming languages</td>
        <td>
            <p>Python</p>
        </td>
    </tr>
    <tr>
        <td>Markup languages</td>
        <td>
            <p>CSS</p>
            <p>HTML</p>
            <p>JSON and JSON5</p>
            <p>RELAX NG</p>
            <p>XML</p>
            <p>YAML</p>
        </td>
    </tr>
    <tr>
        <td>Scripting languages</td>
        <td>
            <p>Shell script</p>
        </td>
    </tr>
    <tr>
        <td>Databases and ORM</td>
        <td>
            <p>MongoJS</p>
            <p>MySQL</p>
            <p>Oracle</p>
            <p>PostgreSQL</p>
            <p>SQL</p>
            <p>SQL Server</p>
        </td>
    </tr>
    <tr>
        <td>Frameworks and libraries</td>
        <td>
            <p>Django</p>
            <p>Google App Engine</p>
            <p>Jupyter</p>
            <p>Pyramid</p>
        </td>
    </tr>
</table>

## Try it now

### Analyze a project locally

#### Install project dependencies

For a basic Python project that has no external dependencies, no preliminary steps are required. 

In case the project has external `pip` dependencies, you can set them up using the `bootstrap` field in the `qodana.yaml` file.  
For example, if your project dependencies are specified by the `requirements.txt` file in your project root, add the following line to `qodana.yaml`:

```yaml
bootstrap: pip install -r requirements.txt
```

The command will be automatically executed before the analysis.

#### Run analysis

<p><include src="lib_qd.xml" include-id="qodana-cli-quickstart" use-filter="non-php,py-only,non-gs,empty"/></p>

## Next steps

- <a href="qodana-python-docker-readme.xml">Configure %linter% Docker image</a>
- <a href="github.md">Run %linter% on GitHub</a>
- <a href="service.md">Use %linter% as a Service</a>
- <a href="ci.md">Extend your CI/CD with %linter% plugins</a>