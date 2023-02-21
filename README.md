# mapping-components-practice

## Why is this important?

A technique called mapping components makes it easy for us to map individual custom pieces of data to custom components.

## Lessons Learned

The map function is a Javascript function that's really useful for handling arrays such as our contacts array (in the repository).

In the case of this specific repository, we're calling a function and then passing it a function. This is kind of the fundamentals of what you might call functional programming, where instead of passing values around your code, you're passing functions into functions even into functions. You can have many levels of functions being passed around.

Dev Tools is useful for debugging.

## Considerations

React is able to create a virtual DOM that represents the current appearance of your website and for it to be able to efficiently render components for every single component that's being rendered using a loop such as the map function, we will have to give those components a property that has to be called "key". This property has to be something that is unique amongst each of these card components that's being created using this loop.

The key prop has to be spelt exactly as displayed within the repository and it's expected to be that way by React. The value can be a string or it can be a number, but it must be unique across all of the repeated components, so in this case our cards.

The reason is because that key property for each React component is a special property. It's used to ensure the right order of items goes into the tree, so that it can render each of these components efficiently when they're being created from a loop, but it is not something that we can tap into. 

<em>(Note that If we actually wanted to show that id which comes from contacts, what we actually have to do is create our own custom prop for example id = contact.id.)</em>
