new Vue({
  el:"#theroot",
  data: {
     greeting:'Hello from VueJS',
     count: 4,
     email:'',
     petAnimals:[
       {name:'Cat'},
       {name:'dog'},
       {name:'Bird'},
       {name:'fsh'},
       {name:'Turtle'},
       {name:'mice'}
       ],
     newPets:''
  },
  methods: {
    addNew: function() {
    	this.petAnimals.push({name: this.newPets})
      this.newPets =''
    }
  },
  computed:{
  		modify: function(){
      if (this.newPets.length >1){
      	return this.newPets +"d"
      }
      }
  }

})
