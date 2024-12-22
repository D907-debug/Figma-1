# Ex09 Event Registration Web Application
# Date:15/12/24
# AIM:
To design, develop and deploy a web application for event registration.

# DESIGN STEPS:
## Step 1:
Create a new frame.

## Step 2:
Select any one preset size of your choice.

## Step 3:
Select the shapes you need.

## Step 4:
Import images as needed.

## Step 5:
Create pages based on your need and link them.

## Step 6:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# DESIGN TOOL:
Figma

# CODE:
~~~
<style>
.auth-container {
  background-color: rgba(236, 232, 17, 1);
  display: flex;
  max-width: 700px;
  flex-direction: column;
  overflow: hidden;
  align-items: center;
  white-space: nowrap;
  padding: 21px 66px 147px;
  font: 400 64px Inter, sans-serif;
}

.logo-banner {
  aspect-ratio: 6.58;
  object-fit: contain;
  object-position: center;
  width: 100%;
  align-self: stretch;
}

.brand-icon {
  aspect-ratio: 1;
  object-fit: contain;
  object-position: center;
  width: 225px;
  margin-top: 59px;
  max-width: 100%;
}

.auth-btn-login {
  background-color: rgba(247, 8, 8, 1);
  margin-top: 89px;
  width: 217px;
  max-width: 100%;
  overflow: hidden;
  color: rgba(246, 239, 239, 1);
  padding: 0 17px 32px;
  cursor: pointer;
}

.auth-btn-register {
  background-color: rgba(239, 23, 23, 1);
  margin-top: 42px;
  width: 337px;
  max-width: 100%;
  overflow: hidden;
  color: rgba(254, 246, 246, 1);
  padding: 0 22px 10px;
  cursor: pointer;
}

@media (max-width: 991px) {
  .auth-container {
    font-size: 40px;
    white-space: initial;
    padding: 0 20px 100px;
  }

  .logo-banner {
    max-width: 100%;
  }

  .brand-icon {
    margin-top: 40px;
  }

  .auth-btn-login {
    font-size: 40px;
    padding-right: 20px;
    margin-top: 40px;
    white-space: initial;
  }

  .auth-btn-register {
    font-size: 40px;
    padding-left: 20px;
    margin-top: 40px;
    white-space: initial;
  }
}
</style>

<div class="auth-container">
  <img
    loading="lazy"
    src="https://cdn.builder.io/api/v1/image/assets/3cecf323b247430885ad254a7e15490c/c32fb45b7551a6764f43711b6bf80d70526096d7f1fb975b65f618d3ccd1e61a?apiKey=3cecf323b247430885ad254a7e15490c&"
    class="logo-banner"
    alt="Company logo banner"
  />
  <img
    loading="lazy"
    src="https://cdn.builder.io/api/v1/image/assets/3cecf323b247430885ad254a7e15490c/1afa5e9a97b67c86f0740ac4942f3a66d35bec4b89ea303548b96363df72b961?apiKey=3cecf323b247430885ad254a7e15490c&"
    class="brand-icon"
    alt="Brand icon"
  />
  <button class="auth-btn-login" tabindex="0">LOGIN</button>
  <button class="auth-btn-register" tabindex="0">REGISTER</button>
</div>
~~~
~~~
<style>
  .sports-events-container {
    background-color: rgba(237, 255, 41, 1);
    display: flex;
    max-width: 700px;
    flex-direction: column;
    overflow: hidden;
    font-family: Inter, sans-serif;
    font-weight: 400;
    padding: 62px 50px;
  }

  .sports-events-title {
    color: rgba(247, 47, 47, 1);
    font-size: 36px;
    align-self: center;
  }

  .sports-events-list {
    color: rgba(0, 0, 0, 1);
    font-size: 24px;
    align-self: start;
    margin-top: 81px;
  }

  @media (max-width: 991px) {
    .sports-events-container {
      padding: 0 20px;
    }

    .sports-events-list {
      margin-top: 40px;
    }
  }
</style>

<div class="sports-events-container" role="region" aria-label="Sports Day Events">
  <h1 class="sports-events-title">SPORTS DAY EVENTS</h1>
  <div class="sports-events-list">
    CRICKET
    <br />
    <br />
    TENNIS
    <br />
    <br />
    BATMINTON
    <br />
    <br />
    VOLLEY BALL
    <br />
    <br />
    KABBADI
    <br />
    <br />
    THROW BALL
    <br />
    <br />
    ARM BALL
    <br />
    <br />
    100 METERS
    <br />
    <br />
    200 METERS
    <br />
    <br />
    400 METERS
    <br />
    <br />
    4-1500 METERS RELAY
  </div>
</div>
~~~
~~~
<style>
  .visually-hidden {
    clip: rect(0 0 0 0);
    clip-path: inset(50%);
    height: 1px;
    overflow: hidden;
    position: absolute;
    white-space: nowrap;
    width: 1px;
  }
  
  .registration-container {
    background-color: rgba(236, 232, 17, 1);
    display: flex;
    max-width: 700px;
    flex-direction: column;
    overflow: hidden;
    align-items: start;
    color: rgba(0, 0, 0, 1);
    padding: 86px 48px 13px;
    font: 400 24px Inter, sans-serif;
  }
  
  .form-title {
    color: rgba(83, 69, 190, 1);
    font-size: 36px;
    align-self: end;
  }
  
  .input-field {
    background-color: rgba(255, 255, 255, 1);
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: none;
  }
  
  .name-field {
    width: 519px;
    max-width: 100%;
  }
  
  .gender-field {
    width: 355px;
    max-width: 100%;
  }
  
  .age-reg-container {
    display: flex;
    margin-top: 35px;
    width: 100%;
    max-width: 570px;
    gap: 40px 66px;
    flex-wrap: wrap;
  }
  
  .department-field {
    width: 387px;
    max-width: 100%;
    margin-left: 10px;
  }
  
  .contact-field {
    width: 362px;
    max-width: 100%;
    margin-left: 22px;
  }
  
  .events-field {
    width: 353px;
    max-width: 100%;
    margin: 25px 0 0 10px;
  }
  
  .submit-button {
    background-color: rgba(142, 111, 111, 1);
    color: rgba(174, 18, 18, 1);
    border: none;
    width: 201px;
    padding: 11px 45px;
    margin: 47px auto 0;
    cursor: pointer;
  }
  
  @media (max-width: 991px) {
    .registration-container {
      padding: 0 20px;
    }
    
    .form-title {
      max-width: 100%;
    }
    
    .name-field {
      padding-right: 20px;
      margin-top: 40px;
    }
    
    .gender-field {
      padding-right: 20px;
    }
    
    .age-reg-container {
      max-width: 100%;
    }
    
    .department-field {
      padding-right: 20px;
      margin-top: 40px;
    }
    
    .contact-field {
      margin-left: 10px;
      padding-right: 20px;
    }
    
    .events-field {
      padding: 0 20px;
    }
    
    .submit-button {
      margin-top: 40px;
      padding: 0 20px;
    }
  }
</style>

<form class="registration-container">
  <h1 class="form-title">EVENT REGISTRATION FORM</h1>
  
  <label for="fullName" class="visually-hidden">Full Name</label>
  <input type="text" id="fullName" class="input-field name-field" placeholder="FULL NAME:" required>
  
  <label for="gender" class="visually-hidden">Gender</label>
  <select id="gender" class="input-field gender-field" required>
    <option value="">GENDER:</option>
    <option value="male">Male</option>
    <option value="female">Female</option>
    <option value="other">Other</option>
  </select>
  
  <div class="age-reg-container">
    <div>
      <label for="age" class="visually-hidden">Age</label>
      <input type="number" id="age" class="input-field" placeholder="AGE:" required>
    </div>
    <div>
      <label for="regNo" class="visually-hidden">Registration Number</label>
      <input type="text" id="regNo" class="input-field" placeholder="REG NO:" required>
    </div>
  </div>
  
  <label for="department" class="visually-hidden">Department</label>
  <input type="text" id="department" class="input-field department-field" placeholder="DEPARTMENT:" required>
  
  <label for="mobile" class="visually-hidden">Mobile Number</label>
  <input type="tel" id="mobile" class="input-field contact-field" placeholder="MOBILE NO:" required>
  
  <label for="email" class="visually-hidden">Email ID</label>
  <input type="email" id="email" class="input-field contact-field" placeholder="EMAIL ID:" required>
  
  <label for="events" class="visually-hidden">Events to Register</label>
  <select id="events" class="input-field events-field" multiple required>
    <option value="">EVENTS TO REGISTER:</option>
    <option value="event1">Event 1</option>
    <option value="event2">Event 2</option>
    <option value="event3">Event 3</option>
  </select>
  
  <button type="submit" class="submit-button">REGISTER</button>
</form>
~~~
~~~
<style>
  .visually-hidden {
    clip: rect(0 0 0 0);
    clip-path: inset(50%);
    height: 1px;
    overflow: hidden;
    position: absolute;
    white-space: nowrap;
    width: 1px;
  }

  .registration-success {
    background-color: rgba(237, 255, 41, 1);
    display: flex;
    max-width: 700px;
    flex-direction: column;
    overflow: hidden;
    color: rgba(46, 13, 13, 1);
    padding: 34px 29px 458px 77px;
    font: 400 40px Inter, sans-serif;
  }

  .registration-logo {
    aspect-ratio: 6.58;
    object-fit: contain;
    object-position: center;
    width: 100%;
  }

  .registration-message {
    align-self: center;
    margin-top: 180px;
  }

  @media (max-width: 991px) {
    .registration-success {
      padding: 0 20px 100px;
    }

    .registration-logo {
      max-width: 100%;
    }

    .registration-message {
      margin-top: 40px;
    }
  }
</style>

<div class="registration-success">
  <img
    loading="lazy"
    src="https://cdn.builder.io/api/v1/image/assets/3cecf323b247430885ad254a7e15490c/c32fb45b7551a6764f43711b6bf80d70526096d7f1fb975b65f618d3ccd1e61a?apiKey=3cecf323b247430885ad254a7e15490c&"
    class="registration-logo"
    alt="Registration success logo"
  />
  <div class="registration-message" role="status" aria-live="polite">THANK YOU FOR REGISTRATION</div>
</div>
~~~

# OUTPUT:
![image](https://github.com/user-attachments/assets/18978bb7-b1f3-408f-81e1-c9964ec3284a)

# RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
