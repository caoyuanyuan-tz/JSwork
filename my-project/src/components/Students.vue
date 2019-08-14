<template>
    <div>
        <table>
    		<tr v-for="stu in students">
    			<td>{{stu.id}}</td>
    			<td>{{stu.name}}</td>
    		</tr>
    	</table>
    </div>
</template>

<script>
    export default{
        props:{
            students:{
                type:Array,
                default:{{id:1,name:'xxx'}}
            }
        },
        methods:{
            showStu(stu){
                console.log('students',stu)
            }
        }
    }
</script>