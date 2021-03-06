# GlobalizationTranslator

[简体中文](README_zh_CN.md)

Intellij platform i18n plugin，Auto translate 131 languages for your application with one click，Support Android strings.xml and java .properties file

This plugin supports translate Android.xml and java .properties file, which can preserve the placeholders such as ```%1$s```, ```%2$d```, ```{0}```,```{1}``` and can Reserved escape characters like ```\n```,```\"```,```\'```, etc., support ```string```, ```string-array```, ```plurals``` tag.

Advantages of this plugin compared to other plugins: fast translation speed, translate files into 131 languages in less than two minutes, support for retaining placeholders, support for incremental translation.

<h3>Install</h3>

~~Intellij platform -> Settings -> Plugins -> Marketplace -> Search "GlobalizationTranslator" -> Install~~ (Plugin is under review)

Download GlobalizationTranslator.zip from here: [release](https://github.com/wilinz/globalization-translator/releases) -> Settings -> Plugins -> Click Settings Icon Button  -> Install Plugin form Disk

Dependency：<a href="https://plugins.jetbrains.com/plugin/18439-compose-for-ide-plugin-development-experimental-">Compose for IDE Plugin Development (Experimental)</a>
<h4>Download Dependency:</h4>

<ul>
    <li>
        <h4>
            Intellij Version >= 213:
        </h4>
        Settings -> Plugins -> Marketplace -> Search "Compose for IDE Plugin Development (Experimental)" -> Install
    </li>
    <li>
        <h4>
            Intellij Version < 213:
        </h4>
        <a href="https://github.com/wilinz/globalization-translator/releases/download/1.0.0/Compose_Intellij_Plugin_Base-0.1.0.zip">Click here Download</a>
        -> Settings -> Plugins -> Click Settings Icon Button  -> Install Plugin form Disk
    </li>
</ul>

<h2>Usage:</h2>
<h3>1. Translate the entire document</h3>
<ol>
    <li>Select the values/strings.xml or .properties file</li>
    <li>Right click and select "Translate this file".</li>
    <li>Select the languages to be translated.</li>
    <li>Click OK.</li>
</ol>
<h3>2. Incremental translation</h3>
<ol>
    <li>In the values/strings.xml or .properties file, select n lines of content you want to translate</li>
    <li>Right click and select "Translate to Other Languages".</li>
    <li>Select the languages to be translated.</li>
    <li>Click OK.</li>
</ol>

# Announcement

Be careful to choose the source language correctly, otherwise the translation may not be accurate

1.For Android strings.xml please add translatable="false" for strings not to be translated:
```xml
<string name="test" translatable="false">Test</string>
```
2.For .properties file，please store untranslated strings and translated strings in separate files

# Support
https://github.com/wilinz/Sponsor

# Develop：
Run command in terminal: `./gradlew runIde`

<img src="img/20220417014525.png"   />
<img src="img/20220417014733.png"  />
<img src="img/20220417014758.png"   />
