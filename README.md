# Prompt Notes

## Level 1

Writing directly with few details.

- “HTML, CSS, JAVASCRIPT and TAILWIND: Create a retro snake game”
- in xml: count to 10 then back to 0
- EXCLUSIVELY output a sqlite table: User: {id, email, address, isMember}

## Level 2

Writing in XML format in a detailed way. 

- Example 1 : Snake Game
    
    ```xml
    <persona>
        You are a senior software developer. You are an expert in HTML CSS and JAVASCRIPT. You use tailwind with CSS.
    </persona>
    
    <purpose>
        Create a snake game using HTML, CSS and JAVASCRIPT with tailwind.
    </purpose>
    
    <instructions>
        <instruction>
            Create a canvas element with a width of 512px and a height of 512px.
        </instruction>
        <instruction>
            Before the game starts, look for the start button in the center of the canvas. When the game is in progress, there will be a scoreboard in the upper right corner. A restart button when the game is lost. Make sure you check the situations correctly.
        </instruction>
        <instruction>
            Create a snake object that has a length of 3 and a direction of right.
        </instruction>
        <instruction>
            Create a food object that has a random position on the canvas. When the snake eats the food, the snake grows longer. Every time the snake eats the food, the score increases by 1. and the food position is changed to a new random position.
            The snake grows by 1 unit each time it eats.
        </instruction>
        <instruction>
            The game is lost when the snake hits itself.
        </instruction>
        <instruction>
            The snake moves 1 unit at a time. Adjust the unit size according to the size of the canvas. The canvas should have a total of 256 units.
        </instruction>
        <instruction>
            The snake can move up, down, left and right.
        </instruction>
        <instruction>
            Control the snake with the arrow keys.
        </instruction>
        <instruction>
            The game is won when the snake reaches the size of the canvas.
        </instruction>
        <instruction>
            Use retro colors and style for the game.
        </instruction>
    </instructions>
    
    <!-- Bug fix
    <persona>
        You are a senior software developer. You are an expert in HTML CSS and JAVASCRIPT. You use tailwind with CSS.
    </persona>
    
    <purpose>
        Fix the snake game using HTML, CSS and JAVASCRIPT with tailwind. The game is not working as expected.
    </purpose>
    
    <instructions>
        <instruction>
            When I click the start button, the game should start. Now it is not working. Getting an error.
            <error>
                game.js:154 Uncaught SyntaxError: Identifier 'gameLoop' has already been declared
            </error>
        </instruction>
    </instructions>
    -->
    <!-- Update
    <persona>
        You are a senior software developer. You are an expert in HTML CSS and JAVASCRIPT. You use tailwind with CSS.
    </persona>
    
    <purpose>
        Update the snake game using HTML, CSS and JAVASCRIPT with tailwind.
    </purpose>
    
    <instructions>
        <instruction>
            The game is lost when the snake hits the walls. Change this so that the snake can pass through the walls.
        </instruction>
    </instructions>
    -->
    ```
    
- Example 2: Typescript to SQL Table
    
    ```xml
    <persona>
        You are a senior software developer. You are an expert in SQL and typescript.
    </persona>
    
    <purpose>
        Convert the typescript interface to a SQL table definition.
    </purpose>
    
    <instructions>
        <instruction> Use postgres dialect. </instruction>
        <instruction> Respond only with the table definition. </instruction>
        <instruction> Optimize the table for performance. </instruction>
    </instructions>
    
    <interface>
        Users {
        id: number;
        name: string;
        email: string;
        created_at: Date;
        }
    </interface>
    ```
    

## Level 3

Write in detail in XML format and add examples.

- Example: login page
    
    ```xml
    <persona>
        You are a senior software developer. You are an expert in HTML CSS and JAVASCRIPT. You use
        tailwind with CSS.
    </persona>
    
    <purpose>
        Create a login page using HTML, CSS and JAVASCRIPT with tailwind.
    </purpose>
    
    <examples>
        <example>
            <!-- Tailwind example -->
            <!-- tailwind.config.js
                tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            primary:
            {"50":"#eff6ff","100":"#dbeafe","200":"#bfdbfe","300":"#93c5fd","400":"#60a5fa","500":"#3b82f6","600":"#2563eb","700":"#1d4ed8","800":"#1e40af","900":"#1e3a8a","950":"#172554"}
          }
        },
        fontFamily: {
          'body': [
        'Inter', 
        'ui-sans-serif', 
        'system-ui', 
        '-apple-system', 
        'system-ui', 
        'Segoe UI', 
        'Roboto', 
        'Helvetica Neue', 
        'Arial', 
        'Noto Sans', 
        'sans-serif', 
        'Apple Color Emoji', 
        'Segoe UI Emoji', 
        'Segoe UI Symbol', 
        'Noto Color Emoji'
      ],
          'sans': [
        'Inter', 
        'ui-sans-serif', 
        'system-ui', 
        '-apple-system', 
        'system-ui', 
        'Segoe UI', 
        'Roboto', 
        'Helvetica Neue', 
        'Arial', 
        'Noto Sans', 
        'sans-serif', 
        'Apple Color Emoji', 
        'Segoe UI Emoji', 
        'Segoe UI Symbol', 
        'Noto Color Emoji'
      ]
        }
      }
    }
            
            
             -->
            <!-- 
            <section class="bg-gray-50 dark:bg-gray-900">
      <div class="flex flex-col items-center justify-center px-6 py-8 mx-auto md:h-screen lg:py-0">
          <a href="#" class="flex items-center mb-6 text-2xl font-semibold text-gray-900 dark:text-white">
              <img class="w-8 h-8 mr-2" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/logo.svg"
            alt="logo">
              Flowbite    
          </a>
          <div class="w-full bg-white rounded-lg shadow dark:border md:mt-0 sm:max-w-md xl:p-0
            dark:bg-gray-800 dark:border-gray-700">
              <div class="p-6 space-y-4 md:space-y-6 sm:p-8">
                  <h1 class="text-xl font-bold leading-tight tracking-tight text-gray-900 md:text-2xl
            dark:text-white">
                      Sign in to your account
                  </h1>
                  <form class="space-y-4 md:space-y-6" action="#">
                      <div>
                          <label for="email" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Your
            email</label>
                          <input type="email" name="email" id="email" class="bg-gray-50 border border-gray-300 text-gray-900
            rounded-lg focus:ring-primary-600 focus:border-primary-600 block w-full p-2.5
            dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white
            dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="name@company.com"
            required="">
                      </div>
                      <div>
                          <label for="password" class="block mb-2 text-sm font-medium text-gray-900
            dark:text-white">Password</label>
                          <input type="password" name="password" id="password" placeholder="••••••••" class="bg-gray-50
            border border-gray-300 text-gray-900 rounded-lg focus:ring-primary-600
            focus:border-primary-600 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600
            dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500
            dark:focus:border-blue-500" required="">
                      </div>
                      <div class="flex items-center justify-between">
                          <div class="flex items-start">
                              <div class="flex items-center h-5">
                                <input id="remember" aria-describedby="remember" type="checkbox" class="w-4 h-4 border
            border-gray-300 rounded bg-gray-50 focus:ring-3 focus:ring-primary-300 dark:bg-gray-700
            dark:border-gray-600 dark:focus:ring-primary-600 dark:ring-offset-gray-800" required="">
                              </div>
                              <div class="ml-3 text-sm">
                                <label for="remember" class="text-gray-500 dark:text-gray-300">Remember me</label>
                              </div>
                          </div>
                          <a href="#" class="text-sm font-medium text-primary-600 hover:underline
            dark:text-primary-500">Forgot password?</a>
                      </div>
                      <button type="submit" class="w-full text-white bg-primary-600 hover:bg-primary-700 focus:ring-4
            focus:outline-none focus:ring-primary-300 font-medium rounded-lg text-sm px-5 py-2.5
            text-center dark:bg-primary-600 dark:hover:bg-primary-700 dark:focus:ring-primary-800">Sign
            in</button>
                      <p class="text-sm font-light text-gray-500 dark:text-gray-400">
                          Don’t have an account yet? <a href="#" class="font-medium text-primary-600 hover:underline
            dark:text-primary-500">Sign up</a>
                      </p>
                  </form>
              </div>
          </div>
      </div>
    </section>
            -->
        </example>
        <example>
            <!-- Pure html css javascript example
        <!DOCTYPE html>
            <html>
            <head>
            <meta name="viewport" content="width=device-width, initial-scale=1">
            <style>
            body {font-family: Arial, Helvetica, sans-serif;}
            form {border: 3px solid #f1f1f1;}
    
            input[type=text], input[type=password] {
            width: 100%;
            padding: 12px 20px;
            margin: 8px 0;
            display: inline-block;
            border: 1px solid #ccc;
            box-sizing: border-box;
            }
    
            button {
            background-color: #04AA6D;
            color: white;
            padding: 14px 20px;
            margin: 8px 0;
            border: none;
            cursor: pointer;
            width: 100%;
            }
    
            button:hover {
            opacity: 0.8;
            }
    
            .cancelbtn {
            width: auto;
            padding: 10px 18px;
            background-color: #f44336;
            }
    
            .imgcontainer {
            text-align: center;
            margin: 24px 0 12px 0;
            }
    
            img.avatar {
            width: 40%;
            border-radius: 50%;
            }
    
            .container {
            padding: 16px;
            }
    
            span.psw {
            float: right;
            padding-top: 16px;
            }
    
            /* Change styles for span and cancel button on extra small screens */
            @media screen and (max-width: 300px) {
            span.psw {
                display: block;
                float: none;
            }
            .cancelbtn {
                width: 100%;
            }
            }
            </style>
            </head>
            <body>
    
            <h2>Login Form</h2>
    
            <form action="/action_page.php" method="post">
            <div class="imgcontainer">
                <img src="img_avatar2.png" alt="Avatar" class="avatar">
            </div>
    
            <div class="container">
                <label for="uname"><b>Username</b></label>
                <input type="text" placeholder="Enter Username" name="uname" required>
    
                <label for="psw"><b>Password</b></label>
                <input type="password" placeholder="Enter Password" name="psw" required>
                    
                <button type="submit">Login</button>
                <label>
                <input type="checkbox" checked="checked" name="remember"> Remember me
                </label>
            </div>
    
            <div class="container" style="background-color:#f1f1f1">
                <button type="button" class="cancelbtn">Cancel</button>
                <span class="psw">Forgot <a href="#">password?</a></span>
            </div>
            </form>
    
            </body>
            </html>
    
        -->
    
        </example>
    </examples>
    
    <instructions>
        <instruction>
            Form should be responsive.
        </instruction>
        <instruction>
            Form should be centered on the page.
        </instruction>
        <instruction>
            Have an illustration on the right side and login information on the left side.
        </instruction>
        <instruction>
            Have a corporate login page.
        </instruction>
        <instruction>
            Have a remember me button.
        </instruction>
        <instruction>
            Have a forgot password link.
        </instruction>
        <instruction>
            Have a sign up link.
        </instruction>
    </instructions>
    ```
    

## Level 4

Create prompt templates in XML format.

- Example: retro style login page
    
    ```xml
    <persona>
        You are a senior software developer. You are an expert in HTML CSS and JAVASCRIPT. You use
        tailwind with CSS.
    </persona>
    
    <purpose>
        Create a login page using HTML, CSS and JAVASCRIPT with tailwind.
    </purpose>
    
    <example>
        <html>
            <!DOCTYPE html>
            <html lang="en">
                <head>
                    <meta charset="UTF-8" />
                    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
                    <title>Corporate Login</title>
                    <script src="https://cdn.tailwindcss.com"></script>
                    <script src="./tailwind.config.js"></script>
                    <link
                        href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap"
                        rel="stylesheet"
                    />
                </head>
                <body class="bg-gray-100">
                    <div class="min-h-screen flex items-center justify-center">
                        <div class="max-w-6xl w-full mx-auto p-6">
                            <div class="bg-white rounded-2xl shadow-xl flex flex-col md:flex-row">
                                <!-- Login Form Section -->
                                <div class="w-full md:w-1/2 p-8 lg:p-12">
                                    <div class="mb-8">
                                        <h1 class="text-3xl font-bold text-gray-800 mb-2">
                                            Welcome back
                                        </h1>
                                        <p class="text-gray-600">
                                            Please enter your credentials to sign in
                                        </p>
                                    </div>
    
                                    <form id="loginForm" class="space-y-6">
                                        <div>
                                            <label
                                                for="email"
                                                class="block text-sm font-medium text-gray-700 mb-2"
                                            >Email
                                                address</label>
                                            <input
                                                type="email"
                                                id="email"
                                                name="email"
                                                required
                                                class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                                                placeholder="Enter your email"
                                            />
                                        </div>
    
                                        <div>
                                            <label
                                                for="password"
                                                class="block text-sm font-medium text-gray-700 mb-2"
                                            >
                                                Password</label>
                                            <input
                                                type="password"
                                                id="password"
                                                name="password"
                                                required
                                                class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                                                placeholder="Enter your password"
                                            />
                                        </div>
    
                                        <div class="flex items-center justify-between">
                                            <div class="flex items-center">
                                                <input
                                                    type="checkbox"
                                                    id="remember"
                                                    name="remember"
                                                    class="h-4 w-4 text-blue-600 border-gray-300 rounded focus:ring-blue-500"
                                                />
                                                <label for="remember"
                                                    class="ml-2 block text-sm text-gray-700"
                                                >Remember me</label>
                                            </div>
                                            <a href="#"
                                                class="text-sm text-blue-600 hover:text-blue-800"
                                            >Forgot
                                                password?</a>
                                        </div>
    
                                        <button
                                            type="submit"
                                            class="w-full bg-blue-600 text-white py-3 px-4 rounded-lg hover:bg-blue-700 transition duration-200"
                                        >
                                            Sign in
                                        </button>
    
                                        <p class="text-center text-sm text-gray-600"> Don't have an
                                            account? <a
                                                href="#"
                                                class="text-blue-600 hover:text-blue-800 font-medium"
                                            >Sign
                                            up</a>
                                        </p>
                                    </form>
                                </div>
    
                                <!-- Illustration Section -->
                                <div
                                    class="w-full md:w-1/2 bg-blue-600 rounded-r-2xl p-8 lg:p-12 hidden md:block"
                                >
                                    <div class="h-full flex items-center justify-center">
                                        <div class="text-center text-white">
                                            <!-- Illustration svg-->
                                            <h2 class="text-3xl font-bold mb-4">Welcome to Our Platform</h2>
                                            <p class="text-lg opacity-80">
                                                Securely access your workspace and manage your projects
                                                efficiently.
                                            </p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </body>
            </html>
        </html>
        <tailwind.config.js>
            tailwind.config = {
            theme: {
            extend: {
            colors: {
            blue: {
            50: "#eff6ff",
            100: "#dbeafe",
            200: "#bfdbfe",
            300: "#93c5fd",
            400: "#60a5fa",
            500: "#3b82f6",
            600: "#2563eb",
            700: "#1d4ed8",
            800: "#1e40af",
            900: "#1e3a8a",
            }
            },
            fontFamily: {
            sans: ['Inter', 'ui-sans-serif', 'system-ui', '-apple-system', 'Segoe UI', 'Roboto',
            'Helvetica Neue', 'Arial', 'sans-serif'],
            },
            },
            },
            plugins: [],
            }
        </tailwind.config.js>
        <script>
            document.addEventListener('DOMContentLoaded', function () {
            const loginForm = document.getElementById('loginForm');
            const emailInput = document.getElementById('email');
            const passwordInput = document.getElementById('password');
            const rememberCheckbox = document.getElementById('remember');
            loginForm.addEventListener('submit', function (e) {
            e.preventDefault();
    
            // Basic validation
            if (!emailInput.value || !passwordInput.value) {
            alert('Please fill in all fields');
            return;
            }
    
            // Email validation
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailRegex.test(emailInput.value)) {
            alert('Please enter a valid email address');
            return;
            }
    
            // Here you would typically make an API call to your backend
            console.log('Form submitted', {
            email: emailInput.value,
            password: passwordInput.value,
            remember: rememberCheckbox.checked
            });
    
            // For demo purposes, show success message
            alert('Login successful!');
            });
            });
        </script>
    </example>
    
    <instructions>
        <instruction>Form should be responsive.</instruction>
        <instruction>Form should be centered on the page.</instruction>
        <instruction>Have an illustration on the right side and login information on the left side.</instruction>
        <instruction>Have a corporate login page.</instruction>
        <instruction>Have a remember me button.</instruction>
        <instruction>Have a forgot password link.</instruction>
        <instruction>Have a sign up link.</instruction>
        <instruction>Use illustration-as-svg as illustration </instruction>
        <instruction>Use retro-style for page</instruction>
    </instructions>
    
    <illustration-as-svg>
        <svg
            class="w-48 h-48 mx-auto mb-6"
            viewBox="0 0 24 24"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
        >
            <path
                d="M20 7L12 3L4 7M20 7L12 11M20 7V17L12 21M12 11L4 7M12 11V21M4 7V17L12 21"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
            />
        </svg>
    </illustration-as-svg>
    ```
    

Notes:

Encourage thought-provoking outputs for complex tasks.

- Example: Actor
    
    User: Name a famous movie starring an actor who was born in the year 1956. First brainstorm about some actors and their birth years in <brainstorm> tags, then give your answer.
    
    Output:
    
    ```xml
    Here's a brainstorm of some actors and their birth years:
    
    <brainstorm>
    - Tom Hanks (1956)
    - Denzel Washington (1954)
    - Julia Roberts (1967)
    - Harrison Ford (1942)
    - Meryl Streep (1949)
    </brainstorm>
    
    A famous movie starring an actor born in 1956 is:
    
    Forrest Gump, starring Tom Hanks.
    ```
    

Give GPT an out. This will reduce hallucinations.

- Example: Hippo
    
    User: Who is the heaviest hippo of all time?
    
    Unfortunately, there doesn't seem to be a definitive record for the heaviest hippo of all time. Hippos are known to be one of the largest land animals, but their exact weights can vary significantly.
    
    Some key facts about hippo weights:
    
    - Hippos are generally considered the third-largest land animal after elephants and white rhinos. Adult male hippos typically weigh between 1,500 to 3,200 kg (3,300 to 7,100 lbs).
    - The largest recorded wild hippo was a male shot in Uganda in 1926, which weighed around 3,200 kg (7,055 lbs).
    - In captivity, some exceptionally large hippos have been recorded, but their weights are not always verified. For example, a hippo named Bertha at the Los Angeles Zoo was estimated to weigh over 3,800 kg (8,400 lbs) in the 1990s.
    - However, these claims of record-breaking weights are difficult to confirm, as hippos are challenging to weigh accurately, especially in the wild.
    
    So in summary, while there are reports of exceptionally large hippos, there doesn't seem to be a universally accepted record for the single heaviest hippo of all time. The weights can vary significantly based on factors like age, sex, and habitat conditions.
    
    User: Who is the heaviest hippo of all time? Only answer if you know the answer with certainty.
    
    I do not have definitive information about the heaviest hippo of all time. Hippo weights can vary significantly, and without access to comprehensive records, I cannot state with certainty who the heaviest hippo was. Hippo weights are not as well-documented as some other animals, so I do not want to provide an unverified claim.
    

 it's best practice to have the question at the bottom after any text or document.

To reduce the risk of hallucinations in long texts, ask the GPT to first draw out GPT  evidence and conclusions and then wait for GPT  to reach a conclusion from that evidence and conclusions.

To reduce hallucinations, you can turn down the temperature parameter, which is commonly used in GPTs. In the range 0 to 1.

## Old but gold Claude Complex Prompt Examples:

- Complex Prompt for Financial Services
    
    
    | User: You are a master tax acountant. Your task is to answer user questions using any provided reference documentation.Here is the material you should use to answer the user's question:<docs>(a)General ruleIf, in connection with the performance of services, property is transferred to any person other than the person for whom such services are performed, the excess of—(1)the fair market value of such property (determined without regard to any restriction other than a restriction which by its terms will never lapse) at the first time the rights of the person having the beneficial interest in such property are transferable or are not subject to a substantial risk of forfeiture, whichever occurs earlier, over(2)the amount (if any) paid for such property,shall be included in the gross income of the person who performed such services in the first taxable year in which the rights of the person having the beneficial interest in such property are transferable or are not subject to a substantial risk of forfeiture, whichever is applicable. The preceding sentence shall not apply if such person sells or otherwise disposes of such property in an arm’s length transaction before his rights in such property become transferable or not subject to a substantial risk of forfeiture.(b)Election to include in gross income in year of transfer(1)In generalAny person who performs services in connection with which property is transferred to any person may elect to include in his gross income for the taxable year in which such property is transferred, the excess of—(A)the fair market value of such property at the time of transfer (determined without regard to any restriction other than a restriction which by its terms will never lapse), over(B)the amount (if any) paid for such property.If such election is made, subsection (a) shall not apply with respect to the transfer of such property, and if such property is subsequently forfeited, no deduction shall be allowed in respect of such forfeiture.(2)ElectionAn election under paragraph (1) with respect to any transfer of property shall be made in such manner as the Secretary prescribes and shall be made not later than 30 days after the date of such transfer. Such election may not be revoked except with the consent of the Secretary.(c)Special rulesFor purposes of this section—(1)Substantial risk of forfeitureThe rights of a person in property are subject to a substantial risk of forfeiture if such person’s rights to full enjoyment of such property are conditioned upon the future performance of substantial services by any individual.(2)Transferability of propertyThe rights of a person in property are transferable only if the rights in such property of any transferee are not subject to a substantial risk of forfeiture.(3)Sales which may give rise to suit under section 16(b) of the Securities Exchange Act of 1934So long as the sale of property at a profit could subject a person to suit under section 16(b) of the Securities Exchange Act of 1934, such person’s rights in such property are—(A)subject to a substantial risk of forfeiture, and(B)not transferable.(4)For purposes of determining an individual’s basis in property transferred in connection with the performance of services, rules similar to the rules of section 72(w) shall apply.(d)Certain restrictions which will never lapse(1)ValuationIn the case of property subject to a restriction which by its terms will never lapse, and which allows the transferee to sell such property only at a price determined under a formula, the price so determined shall be deemed to be the fair market value of the property unless established to the contrary by the Secretary, and the burden of proof shall be on the Secretary with respect to such value.(2)CancellationIf, in the case of property subject to a restriction which by its terms will never lapse, the restriction is canceled, then, unless the taxpayer establishes—(A)that such cancellation was not compensatory, and(B)that the person, if any, who would be allowed a deduction if the cancellation were treated as compensatory, will treat the transaction as not compensatory, as evidenced in such manner as the Secretary shall prescribe by regulations,the excess of the fair market value of the property (computed without regard to the restrictions) at the time of cancellation over the sum of—(C)the fair market value of such property (computed by taking the restriction into account) immediately before the cancellation, and(D)the amount, if any, paid for the cancellation,shall be treated as compensation for the taxable year in which such cancellation occurs.(e)Applicability of sectionThis section shall not apply to—(1)a transaction to which section 421 applies,(2)a transfer to or from a trust described in section 401(a) or a transfer under an annuity plan which meets the requirements of section 404(a)(2),(3)the transfer of an option without a readily ascertainable fair market value,(4)the transfer of property pursuant to the exercise of an option with a readily ascertainable fair market value at the date of grant, or(5)group-term life insurance to which section 79 applies.(f)Holding periodIn determining the period for which the taxpayer has held property to which subsection (a) applies, there shall be included only the period beginning at the first time his rights in such property are transferable or are not subject to a substantial risk of forfeiture, whichever occurs earlier.(g)Certain exchangesIf property to which subsection (a) applies is exchanged for property subject to restrictions and conditions substantially similar to those to which the property given in such exchange was subject, and if section 354, 355, 356, or 1036 (or so much of section 1031 as relates to section 1036) applied to such exchange, or if such exchange was pursuant to the exercise of a conversion privilege—(1)such exchange shall be disregarded for purposes of subsection (a), and(2)the property received shall be treated as property to which subsection (a) applies.(h)Deduction by employerIn the case of a transfer of property to which this section applies or a cancellation of a restriction described in subsection (d), there shall be allowed as a deduction under section 162, to the person for whom were performed the services in connection with which such property was transferred, an amount equal to the amount included under subsection (a), (b), or (d)(2) in the gross income of the person who performed such services. Such deduction shall be allowed for the taxable year of such person in which or with which ends the taxable year in which such amount is included in the gross income of the person who performed such services.(i)Qualified equity grants(1)In generalFor purposes of this subtitle—(A)Timing of inclusionIf qualified stock is transferred to a qualified employee who makes an election with respect to such stock under this subsection, subsection (a) shall be applied by including the amount determined under such subsection with respect to such stock in income of the employee in the taxable year determined under subparagraph (B) in lieu of the taxable year described in subsection (a).(B)Taxable year determinedThe taxable year determined under this subparagraph is the taxable year of the employee which includes the earliest of—(i)the first date such qualified stock becomes transferable (including, solely for purposes of this clause, becoming transferable to the employer),(ii)the date the employee first becomes an excluded employee,(iii)the first date on which any stock of the corporation which issued the qualified stock becomes readily tradable on an established securities market (as determined by the Secretary, but not including any market unless such market is recognized as an established securities market by the Secretary for purposes of a provision of this title other than this subsection),(iv)the date that is 5 years after the first date the rights of the employee in such stock are transferable or are not subject to a substantial risk of forfeiture, whichever occurs earlier, or(v)the date on which the employee revokes (at such time and in such manner as the Secretary provides) the election under this subsection with respect to such stock.(2)Qualified stock(A)In generalFor purposes of this subsection, the term “qualified stock” means, with respect to any qualified employee, any stock in a corporation which is the employer of such employee, if—(i)such stock is received—(I)in connection with the exercise of an option, or(II)in settlement of a restricted stock unit, and(ii)such option or restricted stock unit was granted by the corporation—(I)in connection with the performance of services as an employee, and(II)during a calendar year in which such corporation was an eligible corporation.(B)LimitationThe term “qualified stock” shall not include any stock if the employee may sell such stock to, or otherwise receive cash in lieu of stock from, the corporation at the time that the rights of the employee in such stock first become transferable or not subject to a substantial risk of forfeiture.(C)Eligible corporationFor purposes of subparagraph (A)(ii)(II)—(i)In generalThe term “eligible corporation” means, with respect to any calendar year, any corporation if—(I)no stock of such corporation (or any predecessor of such corporation) is readily tradable on an established securities market (as determined under paragraph (1)(B)(iii)) during any preceding calendar year, and(II)such corporation has a written plan under which, in such calendar year, not less than 80 percent of all employees who provide services to such corporation in the United States (or any possession of the United States) are granted stock options, or are granted restricted stock units, with the same rights and privileges to receive qualified stock.(ii)Same rights and privilegesFor purposes of clause (i)(II)—(I)except as provided in subclauses (II) and (III), the determination of rights and privileges with respect to stock shall be made in a similar manner as under section 423(b)(5),(II)employees shall not fail to be treated as having the same rights and privileges to receive qualified stock solely because the number of shares available to all employees is not equal in amount, so long as the number of shares available to each employee is more than a de minimis amount, and(III)rights and privileges with respect to the exercise of an option shall not be treated as the same as rights and privileges with respect to the settlement of a restricted stock unit.(iii)EmployeeFor purposes of clause (i)(II), the term “employee” shall not include any employee described in section 4980E(d)(4) or any excluded employee.(iv)Special rule for calendar years before 2018In the case of any calendar year beginning before January 1, 2018, clause (i)(II) shall be applied without regard to whether the rights and privileges with respect to the qualified stock are the same.(3)Qualified employee; excluded employeeFor purposes of this subsection—(A)In generalThe term “qualified employee” means any individual who—(i)is not an excluded employee, and(ii)agrees in the election made under this subsection to meet such requirements as are determined by the Secretary to be necessary to ensure that the withholding requirements of the corporation under chapter 24 with respect to the qualified stock are met.(B)Excluded employeeThe term “excluded employee” means, with respect to any corporation, any individual—(i)who is a 1-percent owner (within the meaning of section 416(i)(1)(B)(ii)) at any time during the calendar year or who was such a 1 percent owner at any time during the 10 preceding calendar years,(ii)who is or has been at any prior time—(I)the chief executive officer of such corporation or an individual acting in such a capacity, or(II)the chief financial officer of such corporation or an individual acting in such a capacity,(iii)who bears a relationship described in section 318(a)(1) to any individual described in subclause (I) or (II) of clause (ii), or(iv)who is one of the 4 highest compensated officers of such corporation for the taxable year, or was one of the 4 highest compensated officers of such corporation for any of the 10 preceding taxable years, determined with respect to each such taxable year on the basis of the shareholder disclosure rules for compensation under the Securities Exchange Act of 1934 (as if such rules applied to such corporation).(4)Election(A)Time for making electionAn election with respect to qualified stock shall be made under this subsection no later than 30 days after the first date the rights of the employee in such stock are transferable or are not subject to a substantial risk of forfeiture, whichever occurs earlier, and shall be made in a manner similar to the manner in which an election is made under subsection (b).(B)LimitationsNo election may be made under this section with respect to any qualified stock if—(i)the qualified employee has made an election under subsection (b) with respect to such qualified stock,(ii)any stock of the corporation which issued the qualified stock is readily tradable on an established securities market (as determined under paragraph (1)(B)(iii)) at any time before the election is made, or(iii)such corporation purchased any of its outstanding stock in the calendar year preceding the calendar year which includes the first date the rights of the employee in such stock are transferable or are not subject to a substantial risk of forfeiture, unless—(I)not less than 25 percent of the total dollar amount of the stock so purchased is deferral stock, and(II)the determination of which individuals from whom deferral stock is purchased is made on a reasonable basis.(C)Definitions and special rules related to limitation on stock redemptions(i)Deferral stockFor purposes of this paragraph, the term “deferral stock” means stock with respect to which an election is in effect under this subsection.(ii)Deferral stock with respect to any individual not taken into account if individual holds deferral stock with longer deferral periodStock purchased by a corporation from any individual shall not be treated as deferral stock for purposes of subparagraph (B)(iii) if such individual (immediately after such purchase) holds any deferral stock with respect to which an election has been in effect under this subsection for a longer period than the election with respect to the stock so purchased.(iii)Purchase of all outstanding deferral stockThe requirements of subclauses (I) and (II) of subparagraph (B)(iii) shall be treated as met if the stock so purchased includes all of the corporation’s outstanding deferral stock.(iv)ReportingAny corporation which has outstanding deferral stock as of the beginning of any calendar year and which purchases any of its outstanding stock during such calendar year shall include on its return of tax for the taxable year in which, or with which, such calendar year ends the total dollar amount of its outstanding stock so purchased during such calendar year and such other information as the Secretary requires for purposes of administering this paragraph.(5)Controlled groupsFor purposes of this subsection, all persons treated as a single employer under section 414(b) shall be treated as 1 corporation.(6)Notice requirementAny corporation which transfers qualified stock to a qualified employee shall, at the time that (or a reasonable period before) an amount attributable to such stock would (but for this subsection) first be includible in the gross income of such employee—(A)certify to such employee that such stock is qualified stock, and(B)notify such employee—(i)that the employee may be eligible to elect to defer income on such stock under this subsection, and(ii)that, if the employee makes such an election—(I)the amount of income recognized at the end of the deferral period will be based on the value of the stock at the time at which the rights of the employee in such stock first become transferable or not subject to substantial risk of forfeiture, notwithstanding whether the value of the stock has declined during the deferral period,(II)the amount of such income recognized at the end of the deferral period will be subject to withholding under section 3401(i) at the rate determined under section 3402(t), and(III)the responsibilities of the employee (as determined by the Secretary under paragraph (3)(A)(ii)) with respect to such withholding.(7)Restricted stock unitsThis section (other than this subsection), including any election under subsection (b), shall not apply to restricted stock units.</docs>Here is an example of how to respond:<example><question>What defines a "qualified" employee?</question><answer><quotes>For purposes of this subsection—(A)In generalThe term "qualified employee" means any individual who—(i)is not an excluded employee, and(ii)agrees in the election made under this subsection to meet such requirements as are determined by the Secretary to be necessary to ensure that the withholding requirements of the corporation under chapter 24 with respect to the qualified stock are met.</quotes><answer>According to the provided documentation, a "qualified employee" is defined as an individual who:1. Is not an "excluded employee" as defined in the documentation.2. Agrees to meet the requirements determined by the Secretary to ensure the corporation's withholding requirements under Chapter 24 are met with respect to the qualified stock.</answer></example>First, gather quotes in <quotes></quotes> tags that are relevant to answering the user's question. If there are no quotes, write "no relevant quotes found".Then insert two paragraph breaks before answering the user question within <answer></answer> tags. Only answer the user's question if you are confident that the quotes in <quotes></quotes> tags support your answer. If not, tell the user that you unfortunately do not have enough information to answer the user's question.Here is the user question: How long do I have to make an 83b election? |
    | --- |
- Answer
    
    
    | <quotes>An election under paragraph (1) with respect to any transfer of property shall be made in such manner as the Secretary prescribes and shall be made not later than 30 days after the date of such transfer. Such election may not be revoked except with the consent of the Secretary.</quotes><answer>According to the documentation, you have 30 days after the date of the property transfer to make an 83(b) election. The election cannot be revoked except with the consent of the Secretary.</answer> |
    | --- |
- Complex Prompt for Legal Services
    
    
    | User: You are an expert lawyer.Here is some research that's been compiled. Use it to answer a legal question from the user.<legal_research><search_results><search_result id=1>The animal health industry became caught up in a number of patent and trademark lawsuits during the past year. In 1994, Barclay Slocum obtained patents for the tibial plateau leveling osteotomy procedure, which is used in the treatment of dogs with cranial cruciate ligament rupture, and for the devices used in the procedure. During 2006, Slocum Enterprises filed a patent infringement suit against New Generation Devices, arguing that the Unity Cruciate Plate manufactured by New Generation infringed on the patent for the Slocum TPLO plate. However, the court never reached a decision on the issue of patent infringement, ruling that it did not have jurisdiction on the basis of the small number of plates sold in the state in which the case was filed and the information provided on a Web site maintained by Slocum Enterprises. Other patent battles waged during 2006 concerned the use of laser technology for onychectomy in cats, pet identification chips, pig vaccines, and pet “deshedding” tools.</search_result><search_result id=2>In Canada, the British Columbia Veterinary Medical Association brought suit against a nonveterinarian, claiming that he engaged in cutting or otherwise removing hooks from horses' teeth and floating horses' teeth with power and manual tools, provided advice and diagnoses in return for a fee, and held himself out as being qualified and willing to provide treatment with respect to these activities. The court held that the intention of the legislature in passing the Veterinary Profession Act was the protection of the public and animals and further held that monopolistic statutes serve the purpose of protecting the public. In addition, the court concluded that dentistry, at its core, relates to the health of the teeth and gums; is distinct from cosmetic and other types of care of animals; and, therefore, falls under the definition of the practice of veterinary medicine. The nonveterinarian was enjoined from providing services without a veterinarian supervising the procedures.</search_result><search_result id=3>The aftermath of Hurricane Katrina, which hit the Gulf Coast of the United States during 2005, spurred changes to the way animals are treated during natural disasters. In 2006, Hawaii, Louisiana, and New Hampshire all enacted laws that address issues regarding the care of animals during disasters, such as providing shelters for pets and allowing service animals to be kept with the people they serve. In addition, Congress passed, and the President signed, the Pet Evacuation and Transportation Standards Act during 2006, which requires state and local emergency preparedness authorities to include in their evacuation plans information on how they will accommodate household pets and service animals in case of a disaster. California passed a law that will require its Office of Emergency Services, Department of Agriculture, and other agencies involved with disaster response preparation to develop a plan for the needs of service animals, livestock, equids, and household pets in the event of a disaster or major emergency.</search_result></search_results></legal_research>When citing the legal research in your answer, please use brackets containing the search index ID, followed by a period. Put these at the end of the sentence that's doing the citing. Examples of proper citation format:<examples><example>The statute of limitations expires after 10 years for crimes like this. [3].</example><example>However, the protection does not apply when it has been specifically waived by both parties. [5].</example></examples>Write a clear, concise answer to this question:<question>Are there any laws about what to do with pets during a hurricane?</question>It should be no more than a couple of paragraphs. If possible, it should conclude with a single sentence directly answering the user's question. However, if there is not sufficient information in the compiled research to produce such an answer, you may demur and write "Sorry, I do not have sufficient information at hand to answer this question.".Before you answer, pull out the most relevant quotes from the research in <relevant_quotes> tags.Put your two-paragraph response in <answer> tags.Assistant: <relevant_quotes> |
    | --- |
- Answer
    
    
    | "In 2006, Hawaii, Louisiana, and New Hampshire all enacted laws that address issues regarding the care of animals during disasters, such as providing shelters for pets and allowing service animals to be kept with the people they serve. In addition, Congress passed, and the President signed, the Pet Evacuation and Transportation Standards Act during 2006, which requires state and local emergency preparedness authorities to include in their evacuation plans information on how they will accommodate household pets and service animals in case of a disaster." [3]"California passed a law that will require its Office of Emergency Services, Department of Agriculture, and other agencies involved with disaster response preparation to develop a plan for the needs of service animals, livestock, equids, and household pets in the event of a disaster or major emergency." [3]</relevant_quotes><answer>The research indicates that there are several laws in place regarding the treatment of pets during natural disasters like hurricanes. In 2006, several states, including Hawaii, Louisiana, and New Hampshire, enacted laws that require shelters to accommodate pets and allow service animals to remain with their owners during evacuations. [3] Additionally, the federal government passed the Pet Evacuation and Transportation Standards Act in 2006, which mandates that state and local emergency preparedness authorities include plans for accommodating household pets and service animals in their disaster response plans. [3] California has also passed a law requiring state agencies to develop plans for addressing the needs of pets, livestock, and other animals during emergencies. [3]In summary, there are now various laws in place that require emergency authorities to make provisions for the care and evacuation of pets during natural disasters like hurricanes.</answer> |
    | --- |
- Complex Prompt for Coding
    
    
    | User: You are Codebot, a helpful AI assistant who finds issues with code and suggests possible improvements.Act as a Socratic tutor who helps the user learn.You will be given some code from a user. Please do the following:1. Identify any issues in the code. Put each issue inside separate <issues> tags.2. Invite the user to write a revised version of the code to fix the issue.Here's an example:<example><code>def calculate_circle_area(radius):    return (3.14 * radius) ** 2</code><issues><issue>3.14 is being squared when it's actually only the radius that should be squared></issue><response>That's almost right, but there's an issue related to order of operations. It may help to write out the formula for a circle and then look closely at the parentheses in your code.</response></example>Here is the code you are to analyze:<code># Function to print multiplicative inversesdef print_multiplicative_inverses(x, n):  for i in range(n):    print(x / i) </code>Find the relevant issues and write the Socratic tutor-style response. Do not give the user too much help! Instead, just give them guidance so they can find the correct solution themselves.Put each issue in <issue> tags and put your final response in <response> tags. |
    | --- |
- Answer
    
    
    | Here is my analysis of the code:<issues><issue>The function `print_multiplicative_inverses` does not actually calculate the multiplicative inverse of `x` with respect to `i`. Instead, it simply prints the result of `x / i`, which is not the multiplicative inverse.</issue><issue>The function does not check if `i` is actually a factor of `x`, which is required for the multiplicative inverse to exist. If `i` is not a factor of `x`, then the multiplicative inverse does not exist.</issue></issues><response>It looks like you're trying to print the multiplicative inverses of `x` with respect to the numbers from 0 to `n-1`. However, the current implementation doesn't quite achieve that. Can you think of how you might need to modify the code to correctly calculate and print the multiplicative inverses? You may want to consider the mathematical definition of a multiplicative inverse and how that relates to the factors of `x`.</response> |
    | --- |

### Resources:

[Prompt engineering overview - Anthropic](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)

[IndyDevDan](https://www.youtube.com/@indydevdan/videos)

[AI Jason](https://www.youtube.com/@AIJasonZ/videos)

[https://docs.google.com/spreadsheets/d/1jIxjzUWG-6xBVIa2ay6yDpLyeuOh_hR_ZB75a47KX_E/edit?gid=869808629#gid=869808629](https://docs.google.com/spreadsheets/d/1jIxjzUWG-6xBVIa2ay6yDpLyeuOh_hR_ZB75a47KX_E/edit?gid=869808629#gid=869808629)
