# iOS9 and iOS12 Demo Day

## Requirements

1. Fork and clone the repository
2. **Add your presentation content**
    1. Slide deck (4 required slides)
    2. Links
    3. Answer all questions 
    4. YouTube demo video (1-2 min max)
3. Polish your Github Code repository
    1. Add screenshots and an overview to your GitHub Code Repository
    2. You should make that repository the "Public Portfolio" for your project
    3. Look at [John Sundell's Splash project](https://github.com/JohnSundell/Splash) for inspiration (code, images, GIFs)
4. Create a pull request (PR) and **tag your TL and Instructor**

## Links

* Github Code: `https://github.com/TroyChristian/mort-calc
* Github Proposal: https://github.com/users/TroyChristian/projects/1
* Trello/Github Project Kanban: https://github.com/users/TroyChristian/projects/1
* Test Flight Signup (Recommended): `<insert beta signup link here>`
* YouTube demo video (Recommended): `<insert video url here>`

## Hero Image
See Git Repo https://github.com/TroyChristian/mort-calc
`

## Questions (Answer indented below)

1. What was your favorite feature to implement? Why?

    `The Date Picker becuase it required some new areas of exploration.

2. What was your #1 obstacle or bug that you fixed? How did you fix it?

    3 segue's point at the same view for conciseness, but they contain diffrent information. Sorting them was trial and error. linking them holds the whole app together. 
  
3. Share a chunk of code (or file) you're proud of and explain why.

     func calculations(mortgage:Mortgage?){
        guard let mort = mortgage else {return}
        var n = mort.term * -12
        
        var div1:Double = mort.interestRate / 100
        var i:Double = div1 / 12
        var p = Double(mort.loan)
        var numerator1:Double = i + 1.0
        var numerator1asDub = Double(numerator1)
        var nAsDub = Double(n)
        var expo = pow(numerator1asDub, nAsDub)
        var numdec = 1.0 - expo
        var bigdaddypaymentday = numdec / i
        var monthlyamount = p / bigdaddypaymentday
        
        var totalNumberOfPayments = Double(n * -1)
        var totalInterestPaid:Double
        var arg = totalNumberOfPayments - bigdaddypaymentday
        totalInterestPaid = arg * monthlyamount
       var totalPayment = totalInterestPaid + Double(p)}
       
       I was proud of identifying the information I had to learn, practicing it with pen and paper (and Python2!) and then commiting it to code. With some inventive variable names to boot. This wasnt a flippancy or a joke however, but a psychological anchor to help me keep my place in the formula.
       
       
  
4. What is your elevator pitch? (30 second description your Grandma or a 5-year old would understand)

    `Math is difficult under pressure, so let a straightforward and discrete mortgage calculator gift you an edge. Else good look with this: P = V[n(1 + n)^t]/[(1 + n)^t - 1] in the middle of a busy and potentially adversarial conversation. 
  
5. What is your #1 feature?

    `The ability to revisit calculations by their unique ID, and to take notes about them. 
  
6. What are you future goals?

   A more streamlined and powerful version of this idea could be something impressive.

## Required Slides (Add your Keynote to your PR)

In Git repo.

## Slide Requirements

1. 50 pt font minimum
2. Be concise — don't write sentences/paragraphs (put these in your slide notes for speaking)
3. 3-6 bullets maximum per slide
4. Do the squint test (can you read the text if you squint, if so, make the font bigger)
6. Images are always welcome
7. Do the Grandma Test (Would your Grandma understand you?)

### Optional Slides

1. Blooper: What's a funny bug or blooper? (screenshots/GIFs please)
2. Revenue Model: If the app was your sole source of income, how would you monetize it?

## Presentation Format

**7 minutes/team**

* 4 minute presentation (5 minute hard cap)
* 3 minutes of questions

We have ~12 teams presenting today — please practice your presentation with a timer (as a team), and make sure you fit within the time limit.

Plan on having one person present the slides and live demo. Please practice your presentation in front of a mirror or with your team 2-5 times. Have the app running and visible (Simulator or QuickTime) so you can quickly transition between slides and live demo.

* App Name / Team Slide (30 seconds)
* Elevator Pitch Slide (30 seconds)
* Your #1 Feature (30 seconds)
* Live Demo (2 minutes)
* Future Goals (30 seconds)
* Questions (3 minutes)
