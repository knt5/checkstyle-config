# checkstyle-config

A personal [Checkstyle](http://checkstyle.sourceforge.net/) config based on google_checks.xml

## Changed rules

### FileTabCharacter

```
  <module name="FileTabCharacter">
    <property name="severity" value="ignore"/>
  </module>
```

### Indentation

```
    <module name="Indentation">
      <property name="basicOffset" value="8"/>
      <property name="caseIndent" value="8"/>
      <property name="throwsIndent" value="8"/>
      <property name="arrayInitIndent" value="8"/>
      <property name="lineWrappingIndentation" value="8"/>
    </module>
```

### CatchParameterName

```
    <module name="CatchParameterName">
      <property name="format" value="^[a-z][a-z0-9]*[a-zA-Z0-9]*$"/>
      <message key="name.invalidPattern" value="Catch parameter name ''{0}'' must match pattern ''{1}''."/>
    </module>
```
