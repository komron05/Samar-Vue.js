<template >
    <ul class="movue-list list-group">
        
        <MovueItem v-for="movue in movues" :movue="movue"/>
    </ul>
</template>

<script>

import MovueItem from "../movue-item/MovueItem.vue"

export default {
    components:{MovueItem},

    data() {
        return {
            movues:[ 
                {
                    name: 'Salom New-York',
                    viewers :9199,
                    favourite:false,
                    like: true,
                },
                {
                    name: 'Super Mane',
                    viewers: 2999,
                    favourite: true,
                    like: false,


                },
                {
                    name: 'Abdulhamid',
                    viewers :12555,
                    favourite: true,
                    like: true,


                },

                {
                    name: 'Uyda Yolgiz',
                    viewers :8129,
                    favourite: false,
                    like: true,


                }
               
            ]
          
        }
    }

}
</script>;
<style scoped>
.movue-list {
      margin-top: 30px;
      padding: 1.5rem;
      border-radius: 15px;
      background-color: #fcfaf5;
      box-shadow:
  0 2.8px 2.2px rgba(0, 0, 0, 0.034),
  0 6.7px 5.3px rgba(0, 0, 0, 0.048),
  0 12.5px 10px rgba(0, 0, 0, 0.06),
  0 22.3px 17.9px rgba(0, 0, 0, 0.072),
  0 41.8px 33.4px rgba(0, 0, 0, 0.086),
  0 100px 80px rgba(0, 0, 0, 0.12)

}    
</style>