<tamplate>
    <div>
         <input class="form-check-input" onclick="" type="checkbox" value="" id="flexCheckDefault">
          <label class="form-check-label item " v-bind:class="{'item-completed':tugasSaya.isDone}" for="flexCheckDefault">{{  tugasSaya.namaTugas}}</label>
    </div>
</tamplate>

<script>
    export default {
        name: 'ItemTugas',
        props: ["tugasSaya"]
    };
</script>

<style scoped>

</style>