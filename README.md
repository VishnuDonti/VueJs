# VueJs

new Vue({
 el : '#app',
 methods : {
    oninput : function(event) {
    
    }
 },
 computed : {
 },
 template : ''
 
});

el -> short cut for element 
el -> 1 -> instructs the vue to find the template inside the dom.

method -> 2 -> method is a function tied to vue instance ,that gets called to somehow respond to user events

directives --> adds special behaviours to the tags.

v-on:input -> directive -> event handler

v-on -> attach an event handler
input -> event

event.target.value --> target is the input field or any field on which the event occured.

Imperative vs Declarative -->
imperative -->  write our code step by step
Declarative --> rules that application should follow. has a state then follow the states.


Vue Cli -> sets up everything 
Babel and Webpack
Webpack. --> combines all files in to single file 
Babel -> allows execution of ES versions even the browser doesnt support it.





computed  ->> consume the method and apply change to the vue template.


data -> Defines Initial state
methods -> defines the different ways our state can change
computed -> Turns data into viewable values.  If you want to change value before rendering just change it on computed.

v-html --> directive --> snippet of html. render it as html.

steps for rendering ->
1. Vue instance is created
2. data is evaluated.
3. method is executed data properties are updated.
4. if data is updated then view will automatically re render.
5. while re rendering it evaluates computed.

template -> should have one root element

Odd n Ends #1
The template need not in html.
Odd n Ends #2
Computed functions needs to be applied if and if only we need change render.
Odd n Ends #3
Interpolated values in templates can have simple javascript expressions.

div has a display property block

import statement,
Add component in template and in the script section

Best practise is to communicate with parent component than sibbling component

pass props when want to communicate parent to child.

when child wants to communicate from child to parent child needs to emit event and parent will use that event.
$emit --> emit events ('eventName', 'value to be emitted');

npm install --save axios


when working with vue instance data can be object or function
when working with vue component data should be function

v-bind:name(the name accessible from parent component)="". --> :

v-for="key in keys"
:key="" id which is unique for each and every key
v-bind:key=key 

BootStrap expects container on root tag
<img v-bind:src="" />
prop also can be referenced in compute,compute


Vuex --> to handle to data
Vue Router--> different sets of components on screen based on url
Imgur --> Upload Images freely.
Imgur Api to interact with 


Vuex --> handle data

1. State -> holds all of the raw data particular module.
2. Getters -> any operation to be performed on state objects
3. Mutations -> a function that operates on state which makes one distinct operation.
4. Actions -> function that assembles together multiple mutations in a series.

// 
Vue.use(Vuex);

export default new Vuex.Store({
modules : {}
});

store is collection of state, getters, mutations, actions
















