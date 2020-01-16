
Vue.component('fruit-list',{
props:['fruits'],
	template:'<ul> <li v-for="fruit in fruits">{{fruit.name}}</li></ul>' 
}),

Vue.component('healthy-fruits',{
props:['fruits'],
	template:'<ul> <li v-for="fruit in fruits">{{fruit.name}}</li></ul>' 
}),


app = new Vue({
el:'.main',
component:['fruit-list','healthy-fruits'],
data:{
	fruits:[
  	{name:'apple'},
    {name:'banana'},
    {name:'cantaloupe'},
    {name:'guava'}
  
  ],
  newFruit:''
         
  },
  methods:
  {
  addFruits: function(){
  	return this.fruits.push({name:this.newFruit})
  }
  }

})
