# <FunWithFlags.vue />

![](https://media.giphy.com/media/qUlkYKZX6bqvK/giphy.gif)

- Semantic ui
- VueJS

## Overview
Semantic ui provides classes to help render flags by using a combination of either the country name or the country code ex 

```
    <i class"ca flag"></i> OR
    <i class="canada flag></i>
```

Building this component is the easiet part, you can build it your self. This repo majorly helps to build the js file that contains a list of flag objects with their respective key value pairs that holds the code, country and nationality values.

```
    [
        {
            'code': 'ca',
            'country': 'canada',
            'nationality': 'canadian'
        }, {
            'code': 'ng',
            'country': 'nigeria',
            'nationality': 'nigerian'
        }
        ...
    ]
```

If you have not built a select options component before to display flags, then you can follow the example in FunWithFlags component `src/FunWithFlagsComponent.vue` as an example. You only need to provide the flags data as a prop to the component. (See lines 4, 11 and 15 in `src/App.vue`) The js file holding the list of flag objects can be found here `src/flags.js`.

I'll try to ensure that the js file is updated on a regular basis, however you are welcome to contribute to it, copy it whatever the heck you want to do with it just as long as it both helps make your work easier or/and it helps other developers' work easier.

## Hope you have fun with FunWithFlags
![](https://media.giphy.com/media/3ohs83cvmud7ThYTzq/giphy.gif)



## Flags Data Categories
There are a few categories included in this repo. You can choose the source you need by setting the right path `line 11 src/App.vue`

- All (List of flag objects for all countries)
- By continents e.g Africa, Europe, Asia etc
- By regions e.g West African countries, East African countries etc
