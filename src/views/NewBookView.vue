<template>
  <!-- boostrap create a input form two column in a row-->
  <div class="container">
    <form>
      <div class="row">
        <div class="col">
          <label>Title</label>
          <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
            placeholder="Title">
        </div>
        <div class="col">
          <!-- craete a boostrap select list-->
          <label>Category</label>
          <select class="form-select" aria-label="Default select example">
            <option selected>Open this select menu</option>
            <option value="1">Fiction</option>
            <option value="2">Game book</option>
            <option value="3">Animate</option>
          </select>
        </div>
      </div>

      <div class="row">
        <div class="col">
          <label>Author</label>
          <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
            placeholder="Author">
        </div>
        <div class="col">
          <label>Publisher</label>
          <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
            placeholder="publisher">
        </div>
      </div>

      <div class="row">
        <div class="col">
          <label>Year</label>
          <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
            placeholder="year">
        </div>
        <div class="col">
          <label>Location</label>
          <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
            placeholder="Location name in warehouse">
        </div>
      </div>

      <div class="row">


        <div class="col">

          <label>ISBN</label>
          <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
            placeholder="ISBN">

        </div>
        <div class="col">

          <label>Image</label>
          <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
            placeholder="Image URL">
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
      <button type="submit" class="btn btn-primary">Add</button>
    </form>



  </div>


</template>
