# Product Survey Data-Wrangling (Mini Project Pacmann)

The Pacmann product team conducted a product survey and choice-based conjoint analysis to determine the priority of attributes for a new program launch. The attributes they investigated include:

- List of Skills: Create Analytics Dashboard, Create Machine Learning Model, Deploy Machine Learning Model, Design AB Test Experimentation, Perform Customer Lifetime Analysis, Perform Churn Analytics, Perform Credit Scoring Analytics, Perform Customer Segmentation, Perform Price Optimization, and Design Data Pipeline.

- Program Format: Tutorial Based and Mentoring Based.

- Program Price: Rp 250,000.0, Rp 300,000.0, Rp 350,000.0, Rp 400,000.0, Rp 450,000.0, Rp 500,000.0, Rp 550,000.0.

A sample product survey questionnaire can be accessed [here](https://docs.google.com/forms/d/e/1FAIpQLScovDB2pyDd2iefKkQ4_ZB2keYkYaRNsIDRD39KKZee51OS1A/viewform).

The questionnaire was distributed through two channels: organic and used advertisements (ads). Here the data collected from each channel: [organic data](https://docs.google.com/spreadsheets/d/1mDC2RlqFXh6zqtXgjfBZF_WHQ8ECpmb6/edit#gid=1453868824) and [ads data](https://drive.google.com/file/d/1Hf6YCjnRI0YIk0H-IGQKgr3cmBKmVKzO/view).

Here is an example dataset from the survey:
![image](https://github.com/aquemos/Product-Survey-Data-Wrangling---Mini-Project-Pacmann/assets/42811785/52ee131e-3af7-4812-82e7-4cb7bbd99649)

To conduct conjoint analysis, the team requires data in the following format:
![image](https://github.com/aquemos/Product-Survey-Data-Wrangling---Mini-Project-Pacmann/assets/42811785/8d0c3183-5a33-4a0c-b323-ead829de8e41)

Here is an example conversion of a response from one user to question number 1:
![image](https://github.com/aquemos/Product-Survey-Data-Wrangling---Mini-Project-Pacmann/assets/42811785/e85e6093-b376-4d5d-a87f-9ddd5bff3be1)

For example, if a user with the phone number '08xx336019xxx' selects option B for question number 1
![original data](https://github.com/aquemos/Product-Survey-Data-Wrangling---Mini-Project-Pacmann/assets/42811785/0fe2a1be-2e9d-4808-b72f-f04a528acad1)

The value of option B is Perform Customer Segmentation skill. So, the conversion result would be like this:
![conjoint data](https://github.com/aquemos/Product-Survey-Data-Wrangling---Mini-Project-Pacmann/assets/42811785/ce60b1f7-7617-40fc-8525-1642ec448d7d)


Note: that responses are considered invalid if a user selects option D along with other options for the same question. For instance, if a user chooses options 'C' and 'D' for question number 1, this response will be considered invalid and will not be included in the cleaned data.
