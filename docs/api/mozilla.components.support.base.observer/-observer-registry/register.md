[android-components](../../index.md) / [mozilla.components.support.base.observer](../index.md) / [ObserverRegistry](index.md) / [register](./register.md)

# register

`fun register(observer: `[`T`](index.md#T)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/support/base/src/main/java/mozilla/components/support/base/observer/ObserverRegistry.kt#L24)

Overrides [Observable.register](../-observable/register.md)

Registers an observer to get notified about changes.

### Parameters

`observer` - the observer to register.`fun register(observer: `[`T`](index.md#T)`, owner: LifecycleOwner, autoPause: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/support/base/src/main/java/mozilla/components/support/base/observer/ObserverRegistry.kt#L30)

Overrides [Observable.register](../-observable/register.md)

Registers an observer to get notified about changes.

The observer will automatically unsubscribe if the lifecycle of the provided LifecycleOwner
becomes DESTROYED.

### Parameters

`observer` - the observer to register.

`owner` - the lifecycle owner the provided observer is bound to.

`autoPause` - whether or not the observer should automatically be
paused/resumed with the bound lifecycle.`fun register(observer: `[`T`](index.md#T)`, view: `[`View`](https://developer.android.com/reference/android/view/View.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/support/base/src/main/java/mozilla/components/support/base/observer/ObserverRegistry.kt#L48)

Overrides [Observable.register](../-observable/register.md)

Registers an observer to get notified about changes.

The observer will only be notified if the view is attached and will be unregistered/
registered if the attached state changes.

### Parameters

`observer` - the observer to register.

`view` - the view the provided observer is bound to.