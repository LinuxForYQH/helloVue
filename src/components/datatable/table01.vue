<template>

  <table id="example" class="table table-striped table-bordered" cellspacing="0" >

    <thead>
    <tr>
      <th>Name</th>
      <th>Position</th>
      <th>Office</th>
      <th>Age</th>
      <th>Start date</th>
      <th>Salary</th>
    </tr>
    </thead>
    <tfoot>
    <tr>
      <th>Name</th>
      <th>Position</th>
      <th>Office</th>
      <th>Age</th>
      <th>Start date</th>
      <th>Salary</th>
    </tr>
    </tfoot>
    <tbody>
    <tr>
      <td>Tiger Nixon</td>
      <td>System Architect</td>
      <td>Edinburgh</td>
      <td>61</td>
      <td>2011/04/25</td>
      <td>$320,800</td>
    </tr>
    <tr>
      <td>Garrett Winters</td>
      <td>Accountant</td>
      <td>Tokyo</td>
      <td>63</td>
      <td>2011/07/25</td>
      <td>$170,750</td>
    </tr>
    </tbody>
  </table>
</template>

<script>

  import $ from 'jquery';
  import dt from 'datatables.net-bs';

  import 'bootstrap/dist/css/bootstrap.css';
  import 'datatables.net-bs/css/dataTables.bootstrap.css';


  $.DataTable=dt

  export default {
    name: "table01",
    methods: {
      init: function (option) {

        $(document).ready(function () {
          $('#example').DataTable();
        });

      }
    }
  }

</script>

<style scoped>




</style>
