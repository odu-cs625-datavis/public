# Vega-Lite Notes / References

## Vega-Lite vs. Vega-Lite API

If you search the web for Vega-Lite examples, you'll see a couple different styles of coding based on whether you find the code based on JSON-based [Vega-Lite](https://vega.github.io/vega-lite) or on the [Vega-Lite API](https://github.com/vega/vega-lite-api), used by most examples in Observable.

*These examples come from https://github.com/vega/vega-lite-api*

The Vega-Lite API is loaded with
~~~ js
import {vl} from '@vega/vega-lite-api'
~~~

and you'll see code that starts with `vl` :

~~~ js
vl.markBar()
  .data('data/movies.json')
  .encode(
     vl.x().fieldQ('IMDB_Rating').bin(true),
     vl.y().count()
  )
~~~

With regular Vega-Lite, you're writing a JSON specification (or, spec):
~~~js
{
  "mark": "bar",
  "data": {"url": "data/movies.json"},
  "encoding": {
    "x": {
      "bin": true,
      "field": "IMDB_Rating",
      "type": "quantitative"
    },
    "y": {
      "aggregate": "count",
      "type": "quantitative"
    }
  }
}
~~~

For more info about some of the differences between Vega Embed and the Vega-Lite API, see [Working with Vega-Lite](https://observablehq.com/@didoesdigital/working-with-vega-lite). 

## References

[Vega-Lite JSON-based Reference](https://vega.github.io/vega-lite/docs/)
* Use the JSON version of Vega-Lite in Observable with [Vega Embed](https://github.com/vega/vega-embed)
* [Hello Vega-Embed](https://observablehq.com/@vega/hello-vega-embed) - more examples of using Vega Embed in Observable

[Vega-Lite API Reference](https://vega.github.io/vega-lite-api/api/)
* [Charting with Vega-Lite](https://observablehq.com/@observablehq/vega-lite?collection=@observablehq/observable-for-vega-lite)
* [Vega-Lite Chart Types](https://observablehq.com/@observablehq/vega-lite-chart-types)
