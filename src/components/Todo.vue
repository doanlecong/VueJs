<template>
   <div class="row">
        <div class="header">
            {{todo.title}}
        </div>
        <div class="meta">
            {{todo.project}}
        </div> 
        <div class="extra content">
            <span class="right floated edit icon">
                <i class="edit icon"></i>
            </span>
        </div>
    </div>
    <div class="button" v-show="todo.done">
        Completed
    </div>
    <div class="button" v-show="!todo.done">
        Pending
    </div>
    </template>
<script>
export default {
  
}
</script>
<style>

</style>
