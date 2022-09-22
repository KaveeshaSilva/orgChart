<template>
  <vo-basic
    :data="chartData"
    :draggable="true"
    :pan="true"
    :zoom="true"
    :exportButton="true"
  ></vo-basic>
</template>

<script>
import { VoBasic } from "vue-orgchart";

export default {
  components: { VoBasic },

  created() {
    this.chartData = {
      name: "Parent",
      title: "Machin",

      children: [
        {
          name: "Child-1",
          children: [
            { name: "Last_Child-1", children: [{ name: "1" }, { name: "1" }] },
            { name: "Last_Child-2", children: [{ name: "1" }, { name: "1" }] },
          ],
        },

        {
          name: "Child-2",
          children: [
            { name: "Last_Child-1", children: [{ name: "1" }, { name: "1" }] },
            { name: "Last_Child-2", children: [{ name: "1" }, { name: "1" }] },
          ],
        },

        {
          name: "Child-3",
          children: [
            { name: "Last_Child-1", children: [{ name: "1" }, { name: "1" }] },
            { name: "Last_Child-2", children: [{ name: "1" }, { name: "1" }] },
          ],
        },

        /* { 
                    name: 'Child-4' ,
                    children: [
                        { name: 'Last_Child-1', children: [ {name:'1'}, {name:'1'} ]},
                        { name: 'Last_Child-2', children: [ {name:'1'}, {name:'1'} ] }
                    ]
                },    
                
                { 
                    name: 'Child-5',
                    children: [
                        { name: 'Last_Child-1', children: [ {name:'1'}, {name:'1'} ]},
                        { name: 'Last_Child-2', children: [ {name:'1'}, {name:'1'} ]}
                    ]
                },

                {
                    name: 'Child-6',
                    children: [
                        { name: 'Last_Child-1', children: [ {name:'1'}, {name:'1'} ] },
                        { name: 'Last_Child-2', children: [ {name:'1'}, {name:'1'} ] }
                    ]
                } */
      ],
    };
  },
};
</script>

<style lang="scss" src="../style/orgChart.css">
</style>