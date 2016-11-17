# checkstyle-config

A personal [Checkstyle](http://checkstyle.sourceforge.net/) config based on google_checks.xml

## Customized rules

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

### CustomImportOrder

```
    <module name="CustomImportOrder">
      <property name="customImportOrderRules" value="STATIC###STANDARD_JAVA_PACKAGE###SPECIAL_IMPORTS###THIRD_PARTY_PACKAGE"/>
      <property name="specialImportsRegExp" value="org"/>
      <property name="thirdPartyPackageRegExp" value="com"/>
      <property name="sortImportsInGroupAlphabetically" value="true"/>
      <property name="separateLineBetweenGroups" value="true"/>
    </module>
````

### SummaryJavadoc

```
    <module name="SummaryJavadoc">
      <property name="forbiddenSummaryFragments" value="^@return the *|^This method returns |^A [{]@code [a-zA-Z0-9]+[}]( is a )"/>
      <property name="period" value=""/>
    </module>
````

### OperatorWrap

```
    <module name="OperatorWrap">
      <property name="option" value="eol"/>
      <property name="tokens" value="BAND, BOR, BSR, BXOR, DIV, EQUAL, GE, GT, LAND, LE, LITERAL_INSTANCEOF, LOR, LT, MINUS, MOD, NOT_EQUAL, PLUS, QUESTION, SL, SR, STAR "/>
    </module>
```

### LineLength

```
    <module name="LineLength">
      <property name="ignorePattern" value="^\t*|^package.*|^import.*|a href|href|http://|https://|ftp://"/>
      <property name="max" value="120"/>
    </module>
```

### MethodName

```
    <module name="MethodName">
      <property name="format" value="^[a-z][a-z0-9][a-zA-Z0-9]*$"/>
      <message key="name.invalidPattern" value="Method name ''{0}'' must match pattern ''{1}''."/>
    </module>
```

## Custormized config

### localeLanguage

```
  <property name="localeLanguage" value="en"/>
```
