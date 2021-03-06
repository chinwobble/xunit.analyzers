---
title: xUnit2015
description: Do not use typeof expression to check the exception type
category: Assertions
severity: Warning
---

# This is a documentation stub

Please submit a PR with updates to the [appropriate file]({{ site.github.repository_url }}/tree/master/docs/{{ page.relative_path }}) or create an [issue](https://github.com/xunit/xunit/issues) if you see this.

## Cause

A concise-as-possible description of when this rule is violated. If there's a lot to explain, begin with "A violation of this rule occurs when..."

## Reason for rule

Explain why the user should care about the violation.

## How to fix violations

To fix a violation of this rule, [describe how to fix a violation].

## Examples

### Violates

Example(s) of code that violates the rule.

```csharp
Assert.Throws(typeof(InvalidOperationException), () => FunctionThatThrows());
```

### Does not violate

Example(s) of code that does not violate the rule.

```csharp
Assert.Throws<InvalidOperationException>(() => FunctionThatThrows());
```

## How to suppress violations

**If the severity of your analyzer isn't _Warning_, delete this section.**

```csharp
#pragma warning disable xUnit2015 // <Rule name>
#pragma warning restore xUnit2015 // <Rule name>
```
