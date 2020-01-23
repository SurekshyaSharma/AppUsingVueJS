  Vue.component('plan', {
    template: '#plan-template',
    props: {
      name: {
        type: String
      }
    }
  })
  new Vue({
    el: '#app',
    data: {
      plans: [
    	 {name:'The Single'},
       {name:'The Curious'},
       {name:'The Addict'},
       {name:'The Smart'}
       ]
    }
  })
