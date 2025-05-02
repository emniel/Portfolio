<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Insights | John Doe - Data Analyst</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Custom CSS */
        .hero-gradient {
            background: linear-gradient(135deg, #3b82f6 0%, #8b5cf6 100%);
        }
        .skill-bar {
            transition: width 1.5s ease-in-out;
        }
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        .chart-container {
            position: relative;
            height: 300px;
            width: 100%;
        }
        #animatedChart {
            opacity: 0;
            transition: opacity 1s ease-in-out;
        }
    </style>
</head>
<body class="font-sans antialiased text-gray-800 bg-gray-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-sm sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <i class="fas fa-chart-line text-indigo-600 text-2xl mr-2"></i>
                        <span class="text-xl font-bold text-gray-900">DataInsights</span>
                    </div>
                </div>
                <div class="hidden md:ml-6 md:flex md:items-center md:space-x-8">
                    <a href="#home" class="text-indigo-600 px-3 py-2 text-sm font-medium">Home</a>
                    <a href="#about" class="text-gray-500 hover:text-indigo-600 px-3 py-2 text-sm font-medium">About</a>
                    <a href="#skills" class="text-gray-500 hover:text-indigo-600 px-3 py-2 text-sm font-medium">Skills</a>
                    <a href="#projects" class="text-gray-500 hover:text-indigo-600 px-3 py-2 text-sm font-medium">Projects</a>
                    <a href="#contact" class="text-gray-500 hover:text-indigo-600 px-3 py-2 text-sm font-medium">Contact</a>
                </div>
                <div class="-mr-2 flex items-center md:hidden">
                    <button type="button" id="mobile-menu-button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500">
                        <span class="sr-only">Open main menu</span>
                        <i class="fas fa-bars"></i>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-lg">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="block px-3 py-2 text-base font-medium text-indigo-600">Home</a>
                <a href="#about" class="block px-3 py-2 text-base font-medium text-gray-500 hover:text-indigo-600">About</a>
                <a href="#skills" class="block px-3 py-2 text-base font-medium text-gray-500 hover:text-indigo-600">Skills</a>
                <a href="#projects" class="block px-3 py-2 text-base font-medium text-gray-500 hover:text-indigo-600">Projects</a>
                <a href="#contact" class="block px-3 py-2 text-base font-medium text-gray-500 hover:text-indigo-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-gradient text-white py-20 md:py-32">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="md:flex md:items-center md:justify-between">
                <div class="md:w-1/2 mb-10 md:mb-0">
                    <h1 class="text-4xl md:text-5xl font-bold mb-4">John Doe</h1>
                    <h2 class="text-2xl md:text-3xl font-semibold mb-6">Data Analyst | Business Intelligence Expert</h2>
                    <p class="text-lg mb-8 opacity-90">Transforming raw data into actionable insights that drive business growth and informed decision-making.</p>
                    <div class="flex space-x-4">
                        <a href="#contact" class="bg-white text-indigo-600 hover:bg-gray-100 px-6 py-3 rounded-md font-medium transition duration-300">Get In Touch</a>
                        <a href="#projects" class="border border-white text-white hover:bg-white hover:text-indigo-600 px-6 py-3 rounded-md font-medium transition duration-300">View Projects</a>
                    </div>
                </div>
                <div class="md:w-1/2 flex justify-center">
                    <div class="relative w-64 h-64 md:w-80 md:h-80 bg-white rounded-full overflow-hidden shadow-xl">
                        <img src="https://images.unsplash.com/photo-1557862921-37829c853f5a?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" alt="John Doe" class="w-full h-full object-cover">
                        <div class="absolute inset-0 bg-indigo-600 opacity-10"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">About Me</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="md:flex md:items-center md:space-x-12">
                <div class="md:w-1/3 mb-10 md:mb-0">
                    <div class="bg-gray-100 p-6 rounded-lg shadow-sm">
                        <div class="flex items-center mb-4">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-graduation-cap text-indigo-600 text-xl"></i>
                            </div>
                            <h3 class="text-xl font-semibold">Education</h3>
                        </div>
                        <ul class="space-y-4">
                            <li>
                                <h4 class="font-medium">MSc in Data Science</h4>
                                <p class="text-gray-600">Stanford University, 2018</p>
                            </li>
                            <li>
                                <h4 class="font-medium">BSc in Statistics</h4>
                                <p class="text-gray-600">University of California, 2016</p>
                            </li>
                        </ul>
                    </div>
                </div>
                
                <div class="md:w-2/3">
                    <h3 class="text-2xl font-semibold mb-6">Turning Data into Decisions</h3>
                    <p class="text-gray-600 mb-6">With over 5 years of experience in data analysis and business intelligence, I specialize in extracting meaningful insights from complex datasets. My approach combines technical expertise with business acumen to deliver solutions that drive measurable impact.</p>
                    
                    <div class="grid grid-cols-2 md:grid-cols-3 gap-4 mb-8">
                        <div class="bg-gray-50 p-4 rounded-lg text-center">
                            <div class="text-indigo-600 text-3xl font-bold mb-2">50+</div>
                            <div class="text-gray-600">Projects Completed</div>
                        </div>
                        <div class="bg-gray-50 p-4 rounded-lg text-center">
                            <div class="text-indigo-600 text-3xl font-bold mb-2">15+</div>
                            <div class="text-gray-600">Satisfied Clients</div>
                        </div>
                        <div class="bg-gray-50 p-4 rounded-lg text-center">
                            <div class="text-indigo-600 text-3xl font-bold mb-2">10M+</div>
                            <div class="text-gray-600">Data Points Analyzed</div>
                        </div>
                    </div>
                    
                    <p class="text-gray-600">When I'm not crunching numbers, you can find me hiking, reading about emerging technologies, or mentoring aspiring data professionals.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">Technical Skills</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8 mb-12">
                <div>
                    <h3 class="text-xl font-semibold mb-6">Data Analysis & Visualization</h3>
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">Python (Pandas, NumPy)</span>
                                <span class="text-gray-600">95%</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2.5">
                                <div class="skill-bar bg-indigo-600 h-2.5 rounded-full" style="width: 0%" data-width="95%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">SQL</span>
                                <span class="text-gray-600">90%</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2.5">
                                <div class="skill-bar bg-indigo-600 h-2.5 rounded-full" style="width: 0%" data-width="90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">Tableau</span>
                                <span class="text-gray-600">85%</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2.5">
                                <div class="skill-bar bg-indigo-600 h-2.5 rounded-full" style="width: 0%" data-width="85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">Power BI</span>
                                <span class="text-gray-600">80%</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2.5">
                                <div class="skill-bar bg-indigo-600 h-2.5 rounded-full" style="width: 0%" data-width="80%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div>
                    <h3 class="text-xl font-semibold mb-6">Machine Learning & Big Data</h3>
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">Scikit-learn</span>
                                <span class="text-gray-600">85%</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2.5">
                                <div class="skill-bar bg-indigo-600 h-2.5 rounded-full" style="width: 0%" data-width="85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">TensorFlow</span>
                                <span class="text-gray-600">75%</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2.5">
                                <div class="skill-bar bg-indigo-600 h-2.5 rounded-full" style="width: 0%" data-width="75%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">Spark</span>
                                <span class="text-gray-600">70%</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2.5">
                                <div class="skill-bar bg-indigo-600 h-2.5 rounded-full" style="width: 0%" data-width="70%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">Hadoop</span>
                                <span class="text-gray-600">65%</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2.5">
                                <div class="skill-bar bg-indigo-600 h-2.5 rounded-full" style="width: 0%" data-width="65%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="bg-white p-8 rounded-xl shadow-sm">
                <h3 class="text-xl font-semibold mb-6 text-center">Data Visualization Example</h3>
                <div class="chart-container">
                    <canvas id="animatedChart"></canvas>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">Featured Projects</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="project-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <div class="h-48 bg-indigo-100 flex items-center justify-center">
                        <i class="fas fa-chart-pie text-indigo-600 text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Retail Sales Dashboard</h3>
                        <p class="text-gray-600 mb-4">Interactive dashboard analyzing sales trends across multiple regions with predictive analytics.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-indigo-100 text-indigo-800 text-xs px-3 py-1 rounded-full">Power BI</span>
                            <span class="bg-indigo-100 text-indigo-800 text-xs px-3 py-1 rounded-full">SQL</span>
                            <span class="bg-indigo-100 text-indigo-800 text-xs px-3 py-1 rounded-full">DAX</span>
                        </div>
                        <a href="#" class="text-indigo-600 hover:text-indigo-800 font-medium inline-flex items-center">
                            View Project <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="project-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <div class="h-48 bg-blue-100 flex items-center justify-center">
                        <i class="fas fa-robot text-blue-600 text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Customer Churn Prediction</h3>
                        <p class="text-gray-600 mb-4">Machine learning model predicting customer churn with 92% accuracy for telecom company.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Python</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Scikit-learn</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Pandas</span>
                        </div>
                        <a href="#" class="text-blue-600 hover:text-blue-800 font-medium inline-flex items-center">
                            View Project <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="project-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <div class="h-48 bg-purple-100 flex items-center justify-center">
                        <i class="fas fa-shopping-cart text-purple-600 text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">E-commerce Recommendation System</h3>
                        <p class="text-gray-600 mb-4">Collaborative filtering system that increased average order value by 18%.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-purple-100 text-purple-800 text-xs px-3 py-1 rounded-full">Python</span>
                            <span class="bg-purple-100 text-purple-800 text-xs px-3 py-1 rounded-full">TensorFlow</span>
                            <span class="bg-purple-100 text-purple-800 text-xs px-3 py-1 rounded-full">Flask</span>
                        </div>
                        <a href="#" class="text-purple-600 hover:text-purple-800 font-medium inline-flex items-center">
                            View Project <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="#" class="inline-flex items-center px-6 py-3 border border-indigo-600 text-indigo-600 hover:bg-indigo-600 hover:text-white rounded-md font-medium transition duration-300">
                    View All Projects <i class="fas fa-arrow-right ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">Client Testimonials</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-sm">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/43.jpg" alt="Sarah Johnson" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-semibold">Sarah Johnson</h4>
                            <p class="text-gray-600">CEO, RetailCorp</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-6">"John's analysis of our customer data completely transformed our marketing strategy. His insights led to a 30% increase in customer retention within just three months."</p>
                    <div class="flex text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-sm">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael Chen" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-semibold">Michael Chen</h4>
                            <p class="text-gray-600">Director of Analytics, TechSolutions</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-6">"Working with John was a game-changer for our data team. His expertise in predictive modeling helped us identify new revenue opportunities worth millions."</p>
                    <div class="flex text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">Get In Touch</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="md:flex md:space-x-8">
                <div class="md:w-1/2 mb-10 md:mb-0">
                    <h3 class="text-xl font-semibold mb-6">Let's Collaborate</h3>
                    <p class="text-gray-600 mb-8">Have a data challenge you need help with? Interested in working together? Feel free to reach out through the form or connect with me on social media.</p>
                    
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-envelope text-indigo-600"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">Email</h4>
                                <a href="mailto:john.doe@datainsights.com" class="text-indigo-600 hover:text-indigo-800">john.doe@datainsights.com</a>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-phone text-indigo-600"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">Phone</h4>
                                <a href="tel:+15551234567" class="text-indigo-600 hover:text-indigo-800">+1 (555) 123-4567</a>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-map-marker-alt text-indigo-600"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">Location</h4>
                                <p class="text-gray-600">San Francisco, CA</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mt-8">
                        <h4 class="font-medium mb-4">Connect With Me</h4>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-gray-100 hover:bg-indigo-600 hover:text-white w-10 h-10 rounded-full flex items-center justify-center transition duration-300">
                                <i class="fab fa-linkedin-in"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-indigo-600 hover:text-white w-10 h-10 rounded-full flex items-center justify-center transition duration-300">
                                <i class="fab fa-github"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-indigo-600 hover:text-white w-10 h-10 rounded-full flex items-center justify-center transition duration-300">
                                <i class="fab fa-twitter"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-indigo-600 hover:text-white w-10 h-10 rounded-full flex items-center justify-center transition duration-300">
                                <i class="fab fa-kaggle"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <form class="space-y-6">
                        <div>
                            <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Name</label>
                            <input type="text" id="name" name="name" class="w-full px-4 py-3 border border-gray-300 rounded-md focus:ring-indigo-500 focus:border-indigo-500" placeholder="Your name">
                        </div>
                        
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
                            <input type="email" id="email" name="email" class="w-full px-4 py-3 border border-gray-300 rounded-md focus:ring-indigo-500 focus:border-indigo-500" placeholder="Your email">
                        </div>
                        
                        <div>
                            <label for="subject" class="block text-sm font-medium text-gray-700 mb-1">Subject</label>
                            <input type="text" id="subject" name="subject" class="w-full px-4 py-3 border border-gray-300 rounded-md focus:ring-indigo-500 focus:border-indigo-500" placeholder="Subject">
                        </div>
                        
                        <div>
                            <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Message</label>
                            <textarea id="message" name="message" rows="5" class="w-full px-4 py-3 border border-gray-300 rounded-md focus:ring-indigo-500 focus:border-indigo-500" placeholder="Your message"></textarea>
                        </div>
                        
                        <div>
                            <button type="submit" class="w-full bg-indigo-600 hover:bg-indigo-700 text-white px-6 py-3 rounded-md font-medium transition duration-300">
                                Send Message <i class="fas fa-paper-plane ml-2"></i>
                            </button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="md:flex md:items-center md:justify-between">
                <div class="flex items-center mb-6 md:mb-0">
                    <i class="fas fa-chart-line text-indigo-400 text-2xl mr-2"></i>
                    <span class="text-xl font-bold">DataInsights</span>
                </div>
                
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-white">
                        <i class="fab fa-linkedin-in"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white">
                        <i class="fab fa-twitter"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white">
                        <i class="fab fa-kaggle"></i>
                    </a>
                </div>
            </div>
            
            <div class="mt-8 pt-8 border-t border-gray-800">
                <p class="text-gray-400 text-center">&copy; 2023 DataInsights. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Back to Top Button -->
    <button id="backToTop" class="fixed bottom-8 right-8 bg-indigo-600 text-white w-12 h-12 rounded-full flex items-center justify-center shadow-lg opacity-0 invisible transition-all duration-300">
        <i class="fas fa-arrow-up"></i>
    </button>

    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    mobileMenu.classList.add('hidden');
                }
            });
        });
        
        // Animate skill bars when scrolled into view
        const skillBars = document.querySelectorAll('.skill-bar');
        
        function animateSkillBars() {
            skillBars.forEach(bar => {
                const rect = bar.getBoundingClientRect();
                const isVisible = (rect.top <= window.innerHeight * 0.8) && (rect.bottom >= 0);
                
                if (isVisible && !bar.hasAttribute('data-animated')) {
                    const width = bar.getAttribute('data-width');
                    bar.style.width = width;
                    bar.setAttribute('data-animated', 'true');
                }
            });
        }
        
        // Initialize skill bars animation
        window.addEventListener('load', animateSkillBars);
        window.addEventListener('scroll', animateSkillBars);
        
        // Back to top button
        const backToTopButton = document.getElementById('backToTop');
        
        window.addEventListener('scroll', () => {
            if (window.pageYOffset > 300) {
                backToTopButton.classList.remove('opacity-0', 'invisible');
                backToTopButton.classList.add('opacity-100', 'visible');
            } else {
                backToTopButton.classList.remove('opacity-100', 'visible');
                backToTopButton.classList.add('opacity-0', 'invisible');
            }
        });
        
        backToTopButton.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // Animated chart
        function createAnimatedChart() {
            const ctx = document.getElementById('animatedChart').getContext('2d');
            
            // Show chart with fade-in effect
            setTimeout(() => {
                document.getElementById('animatedChart').style.opacity = '1';
            }, 500);
            
            return new Chart(ctx, {
                type: 'bar',
                data: {
                    labels: ['Data Cleaning', 'Exploratory Analysis', 'Visualization', 'Model Building', 'Insights'],
                    datasets: [{
                        label: 'Project Time Allocation (%)',
                        data: [25, 30, 20, 15, 10],
                        backgroundColor: [
                            'rgba(59, 130, 246, 0.7)',
                            'rgba(99, 102, 241, 0.7)',
                            'rgba(139, 92, 246, 0.7)',
                            'rgba(168, 85, 247, 0.7)',
                            'rgba(217, 70, 239, 0.7)'
                        ],
                        borderColor: [
                            'rgba(59, 130, 246, 1)',
                            'rgba(99, 102, 241, 1)',
                            'rgba(139, 92, 246, 1)',
                            'rgba(168, 85, 247, 1)',
                            'rgba(217, 70, 239, 1)'
                        ],
                        borderWidth: 1
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: {
                        y: {
                            beginAtZero: true,
                            max: 35,
                            ticks: {
                                callback: function(value) {
                                    return value + '%';
                                }
                            }
                        }
                    },
                    plugins: {
                        legend: {
                            position: 'top',
                        },
                        tooltip: {
                            callbacks: {
                                label: function(context) {
                                    return context.parsed.y + '%';
                                }
                            }
                        }
                    },
                    animation: {
                        duration: 2000,
                        easing: 'easeOutQuart'
                    }
                }
            });
        }
        
        // Initialize chart when skills section is in view
        const skillsSection = document.getElementById('skills');
        let chartInitialized = false;
        
        function checkChartVisibility() {
            const rect = skillsSection.getBoundingClientRect();
            const isVisible = (rect.top <= window.innerHeight * 0.8) && (rect.bottom >= 0);
            
            if (isVisible && !chartInitialized) {
                createAnimatedChart();
                chartInitialized = true;
                window.removeEventListener('scroll', checkChartVisibility);
            }
        }
        
        window.addEventListener('load', checkChartVisibility);
        window.addEventListener('scroll', checkChartVisibility);
    </script>
</body>
</html>
