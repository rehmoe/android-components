[android-components](../../index.md) / [mozilla.components.concept.engine](../index.md) / [Engine](./index.md)

# Engine

`interface Engine` [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/concept/engine/src/main/java/mozilla/components/concept/engine/Engine.kt#L14)

Entry point for interacting with the engine implementation.

### Properties

| Name | Summary |
|---|---|
| [settings](settings.md) | `abstract val settings: `[`Settings`](../-settings/index.md)<br>Provides access to the settings of this engine. |

### Functions

| Name | Summary |
|---|---|
| [createSession](create-session.md) | `abstract fun createSession(private: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = false): `[`EngineSession`](../-engine-session/index.md)<br>Creates a new engine session. |
| [createSessionState](create-session-state.md) | `abstract fun createSessionState(json: `[`JSONObject`](https://developer.android.com/reference/org/json/JSONObject.html)`): `[`EngineSessionState`](../-engine-session-state/index.md)<br>Create a new [EngineSessionState](../-engine-session-state/index.md) instance from the serialized JSON representation. |
| [createView](create-view.md) | `abstract fun createView(context: `[`Context`](https://developer.android.com/reference/android/content/Context.html)`, attrs: `[`AttributeSet`](https://developer.android.com/reference/android/util/AttributeSet.html)`? = null): `[`EngineView`](../-engine-view/index.md)<br>Creates a new view for rendering web content. |
| [name](name.md) | `abstract fun name(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Returns the name of this engine. The returned string might be used in filenames and must therefore only contain valid filename characters. |
| [speculativeConnect](speculative-connect.md) | `abstract fun speculativeConnect(url: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Opens a speculative connection to the host of [url](speculative-connect.md#mozilla.components.concept.engine.Engine$speculativeConnect(kotlin.String)/url). |

### Inheritors

| Name | Summary |
|---|---|
| [GeckoEngine](../../mozilla.components.browser.engine.gecko/-gecko-engine/index.md) | `class GeckoEngine : `[`Engine`](./index.md)<br>Gecko-based implementation of Engine interface. |
| [ServoEngine](../../mozilla.components.browser.engine.servo/-servo-engine/index.md) | `class ServoEngine : `[`Engine`](./index.md)<br>Servo-based implementation of the Engine interface. |
| [SystemEngine](../../mozilla.components.browser.engine.system/-system-engine/index.md) | `class SystemEngine : `[`Engine`](./index.md)<br>WebView-based implementation of the Engine interface. |
