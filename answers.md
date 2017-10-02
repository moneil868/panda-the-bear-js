profileImage = document.querySelector('.profile-image')
profileImage.src = 'https://placebear.com/g/400/400'

<!-- Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing. -->

portfolioImage = document.querySelector('.portfolio-image')
portfolioImage.firstElementChild.src = 'https://placebear.com/g/325/225'

<!-- Select the heading that says "Panda the Bear" and change it to your own name. -->

h1Name = document.querySelector('h1')
h1Name.innerText = "Marlon O'Neil"

<!-- Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector) -->

employmentSection = document.querySelector('#employment')
employmentHeader = employmentSection.firstElementChild
employmentHeader.innerText = 'Something Else'

<!-- Change the colour of the body. -->

body = document.querySelector('body')
body.style.backgroundColor = 'light-gray'

<!-- Change the colour of each element using the highlight class. Use a for loop to do this. -->

highlight = document.querySelectorAll('.highlight')
highlight.forEach(function(item){ item.style.color = 'red' });

<!-- Change the font family of the h1 to 'monospace'. -->

h1 = document.querySelectorAll('h1')
h1.forEach(function(item){ item.style.fontFamily = 'monospace' });

<!-- Find a way to select the round icons in the sidebar and then change their colour. -->

actionIcons = document.querySelectorAll('.action-icon-bg')
actionIcons.forEach(function(item){ item.style.backgroundColor = 'orange' });


<!-- Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself". -->

contactFormName = document.querySelector('#name')
contactFormName.placeholder = 'Identify Yourself'

<!-- Change the placeholder attribute of the message field to "state your business". -->

contactFormMessage = document.querySelector('#message')
contactFormMessage.placeholder = 'state your business'

<!-- Give the name field a "value" attribute of "your nemesis". -->

contactFormName.value = 'your nemesis'

<!-- Change the value attribute of the email field to "koalathebear@gmail.com". -->

contactFormEmail = document.querySelector('#email')
contactFormEmail.value = 'koalathebear@gmail.com'

<!-- Change the value of the submit button on the contact form to "En garde!". -->

contactFormSubmit = document.querySelector('#submit')
contactFormSubmit.value = 'En garde!'

<!-- We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute). -->

contactFormSubmit.disabled = true

<!-- We should help Panda protect their privacy by erasing their personal details from the sidebar. -->

personalInfo = document.querySelector('.bio-info')
personalInfo.style.display = 'none'

<!-- That drawing of Pikachu is really cute. Let’s duplicate it using cloneNode() and insert it at the bottom of the .portfolio-container using insertAdjacentHTML() or appendChild(). -->

portfolioRightImage = document.querySelector('#right-image')
pikachu = portfolioRightImage.firstElementChild
new_pikachu = pikachu.cloneNode()
portfolioContainer = document.querySelector('.portfolio-container')
portfolioContainer.appendChild(new_pikachu)

<!-- Wow, that was so satisfying I think we should do it 10 more times. Use a for loop to help you do this. -->

for (i = 0; i < 10; i++ ){
  new_pikachu = pikachu.cloneNode()
  portfolioContainer = document.querySelector('.portfolio-container')
  portfolioContainer.appendChild(new_pikachu)
}


<!-- Let’s add a message about when the page was last updated. We'll do this by appending a new <li> element to the <ul> in the sidebar (you might need to refresh the page to bring back the list items that we emptied out earlier). -->

listItem.classList = 'bio-info-item'
bioInfo = document.querySelector('.bio-info')
bioInfo.appendChild(listItem)

<!-- For bonus marks, apply the correct classes to these new elements of yours so the styling is consistent with the rest of the list items. -->

var leftSpan2 = document.createElement('span');
var leftSpan2.innerHTML = Date()
leftSpan2.appendChild(lastUpdated2);
listItem.appendChild(leftSpan2);
