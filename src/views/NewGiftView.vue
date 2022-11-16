<template>
  <!-- boostrap create a input form two column in a row-->
  <div class="container">
    <form>
      <div class="row">
        <div class="col">
          <label>Title</label>
          <input type="text" class="form-control" placeholder="title">
        </div>
        <div class="col">
          <!-- craete a boostrap select list-->
          <label>Category</label>
          <select class="form-select" aria-label="Default select example">
            <option selected>Open this select menu</option>
            <option value="1">Expensive</option>
            <option value="2">Inexpensive</option>
            <option value="3">Cheap</option>
          </select>
        </div>
      </div>

      <div class="row">
        <div class="col">
          <label>Image</label>
          <input type="text" class="form-control" placeholder="Image URL">
        </div>
        <div class="col">
          <label>Amount</label>
          <input type="text" class="form-control" placeholder="4">
        </div>
      </div>

      <div class="row">
        <div class="col">
          <label>Unit Price(HKD)</label>
          <input type="text" class="form-control" placeholder="1000">
        </div>

        <div class="row">
        <div class="col">
          <label>Donated by</label>
          <input type="text" class="form-control" placeholder="1000">
        </div>
      </div>

        <div class="col">
          <label>Location</label>
          <input type="text" class="form-control" placeholder="Location in warehouse">
        </div>
      </div>

      <div class="row">
        <div class="col">

          <label for="exampleFormControlTextarea1">Description</label>
          <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"
            placeholder="Description show on listing page"></textarea>
        </div>
        <div class="col">

          <label for="exampleFormControlTextarea1">remarks</label>
          <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"
            placeholder="Internal remarks"></textarea>

        </div>
      </div>
      <!-- boostrap button -->
      <button type="submit" class="btn btn-primary">Save</button>
    </form>



  </div>


</template>
