<template>

  <table id="table_id">

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
  import dt from 'datatables.net';


  $.Datatable = dt;

  export default {
    name: "table01",
    methods: {
      init: function (aa) {
        console.log(aa)
        $(document).ready(function () {
          $('#table_id').DataTable();
        });
      }
    }
  }
  //@import url("https://cdn.datatables.net/1.10.16/css/jquery.dataTables.min.css");
</script>

<style scoped>

  @import  '../../assets/datatable/css/jquery.dataTables.min.kk.css';



</style>
