# <FunWithFlags.vue />

![](https://media.giphy.com/media/qUlkYKZX6bqvK/giphy.gif)

- Semantic ui
- VueJS

### About
Semantic ui provides classes to help render flags by using a combination of either the country name or the country code ex 

```
    <i class"ca flag"></i> OR
    <i class="canada flag></i>
```

### Usage
Building this component is the easiet part, you can build it your self. This repo only helps to build the js file that contains a list of flag object with key value pairs to store the code, country and nationality.

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
