---
title: CodeSmell - detekt-api
---

[detekt-api](../../index.html) / [io.gitlab.arturbosch.detekt.api](../index.html) / [CodeSmell](./index.html)

# CodeSmell

`open class CodeSmell : `[`Finding`](../-finding/index.html)

A code smell indicates any possible design problem inside a program's source code.
The type of a code smell is described by an [Issue](../-issue/index.html).

If the design problem results from metric violations, a list of [Metric](../-metric/index.html)'s
can describe further the kind of metrics.

If the design problem manifests by different source locations, references to these
locations can be stored in additional [Entity](../-entity/index.html)'s.

### Constructors

| [&lt;init&gt;](-init-.html) | `CodeSmell(issue: `[`Issue`](../-issue/index.html)`, entity: `[`Entity`](../-entity/index.html)`, message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, metrics: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Metric`](../-metric/index.html)`> = listOf(), references: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Entity`](../-entity/index.html)`> = listOf())`<br>A code smell indicates any possible design problem inside a program's source code. The type of a code smell is described by an [Issue](../-issue/index.html). |

### Properties

| [entity](entity.html) | `open val entity: `[`Entity`](../-entity/index.html) |
| [id](id.html) | `open val id: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [issue](issue.html) | `val issue: `[`Issue`](../-issue/index.html) |
| [message](message.html) | `open val message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [metrics](metrics.html) | `open val metrics: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Metric`](../-metric/index.html)`>` |
| [references](references.html) | `open val references: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Entity`](../-entity/index.html)`>` |

### Functions

| [compact](compact.html) | `open fun compact(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Contract to format implementing object to a string representation. |
| [compactWithSignature](compact-with-signature.html) | `open fun compactWithSignature(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Same as [compact](../-compactable/compact.html) except the content should contain a substring which represents this exact findings via a custom identifier. |
| [messageOrDescription](message-or-description.html) | `open fun messageOrDescription(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Explanation why this finding was raised. |
| [toString](to-string.html) | `open fun toString(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Inheritors

| [CorrectableCodeSmell](../-correctable-code-smell/index.html) | `open class CorrectableCodeSmell : `[`CodeSmell`](./index.html)<br>Represents a code smell for that can be auto corrected. |
| [ThresholdedCodeSmell](../-thresholded-code-smell/index.html) | `open class ThresholdedCodeSmell : `[`CodeSmell`](./index.html)<br>Represents a code smell for which a specific metric can be determined which is responsible for the existence of this rule violation. |

