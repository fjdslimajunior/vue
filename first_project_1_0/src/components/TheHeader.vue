<template> 
    <header class="header">       
        <div>
            <div v-for="(obj, index) in todos" 
                v-bind:key="obj.id"
                class="todo-item"
                >
            <img 
                v-if="obj.imgSrc"
                v-bind:src="obj.imgSrc" 
                :alt="obj.imgAlt"
             >    

                {{ index }} - {{ obj.title}}   
                
            
            </div>
        </div>
    </header>
</template>

<script>
    export default{
        name: 'App',
        data() {
            return {
                
                todos: [
                    {
                        "userId": 1,
                        "id": 1,
                        "title": "delectus aut autem",
                        "completed": false,
                        "imgSrc": "https://s2.glbimg.com/-cvTjMUkwcEmy2MhvlU-iD92Jes=/620x455/e.glbimg.com/og/ed/f/original/2019/07/29/photo-riaan-blog-1.jpg",
                        "imgAlt": "Imagem 1 do portifólio!"

                },
                {
                    "userId": 1,
                    "id": 2,
                    "title": "quis ut nam facilis et officia qui",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 3,
                    "title": "fugiat veniam minus",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 4,
                    "title": "et porro tempora",
                    "completed": true
                },
                {
                    "userId": 1,
                    "id": 5,
                    "title": "laboriosam mollitia et enim quasi adipisci quia provident illum",
                    "completed": false
                }
                ]
            }
        }
    }
</script>

<style>
/* .header{
    background-color: #ffffff; 
    border-color: brown;
    border-radius: 2px;
    border: 2px;
    color: aqua;
    font-size: 2.1rem;
    
} */
.todo-item{
    background-color: #000;
    align-items: left;
    margin: 0 0 5px 0;
    /* padding: 3px 6px; */
    color: pink;
    align-items: justify;
}
</style>
