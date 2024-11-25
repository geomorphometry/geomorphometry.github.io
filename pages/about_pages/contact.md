---
layout: page
title: Talk to us
permalink: /contact/
hero_image: "../uploads/img/headers/contact1.jpg"
hero_darken: true
show_sidebar: false
---


#### Use the form below to contact us.  

**If you are sending files for a blog post (markdown files and images), send all as a ZIP file (max. 5MB).**  
<br>

<div class="block">

<form target="_blank" action="https://formsubmit.co/31775363d5b65b3d5ab0d32bb37c6234" method="POST"  enctype="multipart/form-data">
<!-- <input type="hidden" name="_next" value="https://yourdomain.co/thanks.html"> -->
<input type="hidden" name="_subject" value="[Geomorphometry.org] CONTACT - new form submitted!">
<input type="hidden" name="_template" value="table">
<!-- <input type="hidden" name="_cc" value="another@email.com"> -->
<input type="hidden" name="_autoresponse" value="Thank you for contacting the International Society for Geomorphometry.">



<div class="field is-horizontal">
  <div class="field-label is-normal">
    <label class="label">Name</label>
  </div>
  <div class="field-body">
    <div class="field  is-expanded">
      <p class="control is-expanded has-icons-left">
        <input class="input" name="name" id="name" type="text" placeholder="Name" required>
        <span class="icon is-small is-left">
          <i class="fas fa-user"></i>
        </span>
      </p>
    </div>
  </div>
</div>


<div class="field is-horizontal">
  <div class="field-label is-normal">
    <label class="label">Email</label>
  </div>
  <div class="field-body">
    <div class="field  is-expanded">
      <p class="control is-expanded has-icons-left">
        <input class="input" type="email" name="email" placeholder="you@server.com" required>
        <span class="icon is-small is-left">
          <i class="fas fa-envelope"></i>
        </span>
      </p>
    </div>
  </div>
</div>


<div class="field is-horizontal">
  <div class="field-label">
    <label class="label">ISG member</label>
  </div>
  <div class="field-body">
    <div class="field is-narrow">
      <div class="control">
        <label class="radio">
          <input type="radio" name="member" value="yes">
          Yes
        </label>
        <label class="radio">
          <input type="radio" name="member" value="no">
          No
        </label>
      </div>
    </div>
  </div>
</div>


<div class="field is-horizontal">
  <div class="field-label is-normal">
    <label class="label">Subject</label>
  </div>
  <div class="field-body">
    <div class="field is-narrow">
      <div class="control">
        <div class="select is-fullwidth"  name="subject">
          <select>
            <option>Coffee Talks</option>
            <option>Blog post (announcement)</option>
            <option>Blog post (script/dataset)</option>
            <option>Other</option>
            </select>
        </div>
      </div>
    </div>
  </div>
</div>


<div class="field is-horizontal">
  <div class="field-label is-normal">
    <label class="label">Comments</label>
  </div>
  <div class="field-body">
    <div class="field">
      <div class="control">
        <textarea class="textarea" placeholder="Explain how we can help you"  name="comments"></textarea>
      </div>
    </div>
  </div>
</div>


<div class="field is-horizontal">
  <div class="field-label">
    <label class="label">Upload</label>
  </div>
  <div class="field-body">
  <div id="fileUploader" class="file has-name is-fullwidth">
    <label class="file-label">
      <input id="attachment" class="file-input" type="file" name="attachment" accept="application/zip">
      <span class="file-cta">
        <span class="file-icon">
          <i class="fas fa-upload"></i>
        </span>
        <span class="file-label">
          Choose a file
        </span>
      </span>
      <span class="file-name">
        Please select a ZIP file
      </span>
    </label>
  </div>
  </div>
  </div>


<div class="field is-horizontal">
  <div class="field-label">
    <!-- Left empty for spacing -->
  </div>
  <div class="field-body">
    <div class="field">
    <label class="checkbox">
      <input type="checkbox" id="check" name="check_agree" onclick="toggle_submit()" >
      I have read and agree to the <a href="{{site.baseurl}}/guidelines">guidelines</a> for commenting and posting in Geomorphometry.org.
    </label>
    </div>
  </div>
</div>
  

<div class="field is-horizontal">
  <div class="field-label">
    <!-- Left empty for spacing -->
  </div>
  <div class="field-body">
    <div class="field">
        <input class="button" type="submit" id="submit" value="Submit" disabled/>
        <input class="button" type="reset" id="reset" value="Reset">
    </div>
  </div>
</div>


</form>
</div>

<!-- ------------------------------------------------------------ -->



<script>
const ckbox = document.getElementById('check');
const submt = document.getElementById('submit');
const fupr = document.getElementById('fileUploader');
const rst = document.getElementById('reset');
const fileInput = document.querySelector('#fileUploader input[type=file]');


function toggle_submit() {
  if (ckbox.checked == true) {
    // checkbox is checked
    submt.disabled = false;
  } else {
    // checkbox is not checked.
    submt.disabled = true;
  }
}


rst.onclick = () => {
  const fileName = document.querySelector('#fileUploader .file-name');
  fupr.setAttribute("class", "file has-name is-fullwidth")
  fileName.textContent = "Please select a ZIP file";
}

fileInput.onchange = () => {
  if (fileInput.files.length > 0) {
    const fileName = document.querySelector('#fileUploader .file-name');
    if ( /\.(zip)$/i.test(fileInput.files[0].name) === false ) { 
      alert("not a ZIP file!")
      fupr.setAttribute("class", "file has-name is-fullwidth is-warning")
      fileName.textContent = "Please select a ZIP file";
    } else {
      // alert("ok!")
      fileName.textContent = fileInput.files[0].name;
    }
  }
}



</script>



<!-- [https://docs.google.com/forms/d/e/1FAIpQLSdIAXFnc\_ELwuMN0c-AGZn-Nf874XesjqF1B79gBi5JjSqzTA/viewform?usp=sf\_link](https://docs.google.com/forms/d/e/1FAIpQLSdIAXFnc_ELwuMN0c-AGZn-Nf874XesjqF1B79gBi5JjSqzTA/viewform?usp=sf_link) -->
