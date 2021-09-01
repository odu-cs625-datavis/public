# Vega-Lite vs. Vega-Lite API

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

You can use the JSON version of Vega-Lite in Observable with [Vega Embed](https://github.com/vega/vega-embed).  For more information, see [Hello Vega-Embed](https://observablehq.com/@vega/hello-vega-embed).

For more info about some of the differences between Vega Embed and the Vega-Lite API, see [Working with Vega-Lite](https://observablehq.com/@didoesdigital/working-with-vega-lite).  

*For this class, I don't care which you use or if you use a mix of the two.  It's up to you.*
