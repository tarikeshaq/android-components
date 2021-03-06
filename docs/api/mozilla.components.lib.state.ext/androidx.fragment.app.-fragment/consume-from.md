[android-components](../../index.md) / [mozilla.components.lib.state.ext](../index.md) / [androidx.fragment.app.Fragment](index.md) / [consumeFrom](./consume-from.md)

# consumeFrom

`@MainThread @ExperimentalCoroutinesApi fun <S : `[`State`](../../mozilla.components.lib.state/-state.md)`, A : `[`Action`](../../mozilla.components.lib.state/-action.md)`> Fragment.consumeFrom(store: `[`Store`](../../mozilla.components.lib.state/-store/index.md)`<`[`S`](consume-from.md#S)`, `[`A`](consume-from.md#A)`>, block: (`[`S`](consume-from.md#S)`) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/lib/state/src/main/java/mozilla/components/lib/state/ext/Fragment.kt#L28)

Helper extension method for consuming [State](../../mozilla.components.lib.state/-state.md) from a [Store](../../mozilla.components.lib.state/-store/index.md) sequentially in order inside a
[Fragment](#). The [block](consume-from.md#mozilla.components.lib.state.ext$consumeFrom(androidx.fragment.app.Fragment, mozilla.components.lib.state.Store((mozilla.components.lib.state.ext.consumeFrom.S, mozilla.components.lib.state.ext.consumeFrom.A)), kotlin.Function1((mozilla.components.lib.state.ext.consumeFrom.S, kotlin.Unit)))/block) function will get invoked for every [State](../../mozilla.components.lib.state/-state.md) update.

This helper will automatically stop observing the [Store](../../mozilla.components.lib.state/-store/index.md) once the [View](#) of the [Fragment](#) gets
detached. The fragment's lifecycle will be used to determine when to resume/pause observing the
[Store](../../mozilla.components.lib.state/-store/index.md).

