new Vue({
  el:"#theroot",
  data: {
     greeting:'Hello from VueJS',
     count: 4,
     email:'',
     petAnimals:[
       {name:'Cat'},
       {name:'Dog'},
       {name:'Bird'},
       {name:'Fish'},
       {name:'Turtle'},
       {name:'Mice'}
       ],
     NewPets:''
  },
  methods: {
    addNew: function() {
     return this.petAnimals.push({name: this.NewPets})
    }
  }

})
