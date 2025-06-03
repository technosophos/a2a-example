# Example A2A Agent

This is a Spin app written in TypeScript that provides an A2A agent.

* The agent is asynchronous (not streamed)
* It is a one-shot agent, and doesn't use sessions
* It's _definitely_ not production ready

## To Build:

Make sure you have a recent version of Spin and of NPM.

* Clone this repository
* Export your Gemini key to Spin: `export SPIN_VARIABLE_GEMINI_API_KEY=SOME_KEY`
* Run `spin build --up` to build and start a local verison

## To Deploy to Fermyon Wasm Functions"

To deploy to Fermyon Wasm Functions or Fermyon Cloud, you will need an account on one of those services. Then you can use the relevant command:

```
# Fermyon Wasm Functions
$ spin aka deploy --variable gemini_api_key=$SPIN_VARIABLE_GEMINI_API_KEY
# Fermyon Cloud
$ spin cloud deploy --variable gemini_api_key=$SPIN_VARIABLE_GEMINI_API_KEY
```

You can also deploy to [SpinKube](https://www.spinkube.dev/docs/) if you run Kubernetes.
