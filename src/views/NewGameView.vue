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
            <option value="1">PS5</option>
            <option value="2">Switch</option>
            <option value="3">PC</option>
          </select>
        </div>
      </div>

      <div class="row">
        <div class="col">
          <label>Image</label>
          <input type="text" class="form-control" placeholder="Image URL">
        </div>
        <div class="col">
          <label>Publisher</label>
          <input type="text" class="form-control" placeholder="publisher">
        </div>
      </div>

      <div class="row">
        <div class="col">
          <label>Quantity</label>
          <input type="text" class="form-control" placeholder="year">
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
