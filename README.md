<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kamel Rahmoun | Graphic Designer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .work-item:hover .work-overlay {
            opacity: 1;
            transform: translateY(0);
        }
        
        .work-overlay {
            transition: all 0.3s ease;
            opacity: 0;
            transform: translateY(20px);
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -2px;
            left: 0;
            background-color: #667eea;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .active::after {
            width: 100%;
        }
        
        .hamburger {
            transition: all 0.3s ease;
        }
        
        .hamburger.active {
            transform: rotate(90deg);
        }
        
        .mobile-menu {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.5s ease-out;
        }
        
        .mobile-menu.open {
            max-height: 500px;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">
    <!-- Navigation -->
    <nav class="fixed w-full bg-white shadow-md z-50">
        <div class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <div class="text-2xl font-bold text-gray-800">
                    <a href="#" class="flex items-center">
                        <span class="text-indigo-600">KR</span>
                        <span class="ml-2">Kamel Rahmoun</span>
                    </a>
                </div>
                
                <!-- Desktop Navigation -->
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="nav-link active">Home</a>
                    <a href="#about" class="nav-link">About</a>
                    <a href="#work" class="nav-link">Work</a>
                    <a href="#services" class="nav-link">Services</a>
                    <a href="#contact" class="nav-link">Contact</a>
                </div>
                
                <!-- Mobile menu button -->
                <div class="md:hidden">
                    <button id="menu-btn" class="hamburger focus:outline-none">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
            
            <!-- Mobile Navigation -->
            <div id="mobile-menu" class="mobile-menu md:hidden">
                <div class="px-2 pt-2 pb-4 space-y-1">
                    <a href="#home" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-100">Home</a>
                    <a href="#about" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-100">About</a>
                    <a href="#work" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-100">Work</a>
                    <a href="#services" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-100">Services</a>
                    <a href="#contact" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-100">Contact</a>
                </div>
            </div>
        </div>
    </nav>
    
    <!-- Hero Section -->
    <section id="home" class="hero-gradient pt-32 pb-20 md:pt-40 md:pb-32 text-white">
        <div class="container mx-auto px-6 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-12 md:mb-0">
                <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6">
                    Visual Stories <br>That <span class="text-yellow-300">Inspire</span>
                </h1>
                <p class="text-lg md:text-xl mb-8 opacity-90">
                    I'm Kamel Rahmoun, a graphic designer passionate about creating meaningful visual experiences that connect brands with their audiences.
                </p>
                <div class="flex space-x-4">
                    <a href="#work" class="bg-white text-indigo-600 px-6 py-3 rounded-full font-medium hover:bg-gray-100 transition duration-300">
                        View My Work
                    </a>
                    <a href="#contact" class="border-2 border-white px-6 py-3 rounded-full font-medium hover:bg-white hover:text-indigo-600 transition duration-300">
                        Contact Me
                    </a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <div class="relative w-64 h-64 md:w-80 md:h-80 lg:w-96 lg:h-96 bg-white bg-opacity-20 rounded-full overflow-hidden">
                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80" 
                         alt="Kamel Rahmoun" 
                         class="absolute inset-0 w-full h-full object-cover">
                </div>
            </div>
        </div>
    </section>
    
    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">About Me</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/3 mb-10 md:mb-0 flex justify-center">
                    <div class="relative w-64 h-64 md:w-72 md:h-72 rounded-lg overflow-hidden shadow-xl">
                        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80" 
                             alt="Kamel Rahmoun" 
                             class="w-full h-full object-cover">
                    </div>
                </div>
                
                <div class="md:w-2/3 md:pl-12">
                    <h3 class="text-2xl font-semibold mb-6">Crafting Visual Experiences Since 2015</h3>
                    <p class="text-gray-600 mb-6 leading-relaxed">
                        With over 8 years of experience in the design industry, I've had the privilege of working with startups, established brands, and creative agencies to bring their visions to life through compelling visual storytelling.
                    </p>
                    <p class="text-gray-600 mb-8 leading-relaxed">
                        My approach combines strategic thinking with artistic expression to create designs that not only look beautiful but also communicate effectively and drive results.
                    </p>
                    
                    <div class="grid grid-cols-2 gap-6 mb-8">
                        <div class="flex items-center">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-palette text-indigo-600 text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold">Brand Identity</h4>
                                <p class="text-sm text-gray-500">Logo, Visual Systems</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-laptop-code text-indigo-600 text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold">Digital Design</h4>
                                <p class="text-sm text-gray-500">Web, UI/UX, Social Media</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-print text-indigo-600 text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold">Print Design</h4>
                                <p class="text-sm text-gray-500">Packaging, Publications</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-chart-line text-indigo-600 text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold">Marketing Design</h4>
                                <p class="text-sm text-gray-500">Campaigns, Advertising</p>
                            </div>
                        </div>
                    </div>
                    
                    <a href="#" class="inline-flex items-center text-indigo-600 font-medium">
                        Download CV <i class="fas fa-download ml-2"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Work Section -->
    <section id="work" class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Featured Work</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="work-item relative rounded-lg overflow-hidden shadow-lg">
                    <img src="https://images.unsplash.com/photo-1499678329028-101435549a4e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Brand Identity Project" 
                         class="w-full h-64 object-cover">
                    <div class="work-overlay absolute inset-0 bg-indigo-600 bg-opacity-90 flex flex-col justify-center items-center p-6 text-white">
                        <h3 class="text-xl font-bold mb-2">Nova Brand Identity</h3>
                        <p class="text-sm mb-4 text-center">Complete visual identity for a tech startup including logo, color palette, and brand guidelines.</p>
                        <a href="#" class="inline-flex items-center border-2 border-white px-5 py-2 rounded-full text-sm font-medium hover:bg-white hover:text-indigo-600 transition-all duration-300 transform hover:scale-105">
                            View Project <i class="fas fa-external-link-alt ml-2 text-xs"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="work-item relative rounded-lg overflow-hidden shadow-lg">
                    <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Packaging Design" 
                         class="w-full h-64 object-cover">
                    <div class="work-overlay absolute inset-0 bg-indigo-600 bg-opacity-90 flex flex-col justify-center items-center p-6 text-white">
                        <h3 class="text-xl font-bold mb-2">Organic Skincare Packaging</h3>
                        <p class="text-sm mb-4 text-center">Sustainable packaging design for an organic skincare line with custom illustrations.</p>
                        <a href="#" class="border border-white px-4 py-2 rounded-full text-sm hover:bg-white hover:text-indigo-600 transition duration-300">
                            View Project
                        </a>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="work-item relative rounded-lg overflow-hidden shadow-lg">
                    <img src="https://images.unsplash.com/photo-1467232004584-a241de8bcf5d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1469&q=80" 
                         alt="Web Design" 
                         class="w-full h-64 object-cover">
                    <div class="work-overlay absolute inset-0 bg-indigo-600 bg-opacity-90 flex flex-col justify-center items-center p-6 text-white">
                        <h3 class="text-xl font-bold mb-2">Travel Agency Website</h3>
                        <p class="text-sm mb-4 text-center">UI/UX design for a luxury travel agency website with custom illustrations.</p>
                        <a href="#" class="border border-white px-4 py-2 rounded-full text-sm hover:bg-white hover:text-indigo-600 transition duration-300">
                            View Project
                        </a>
                    </div>
                </div>
                
                <!-- Project 4 -->
                <div class="work-item relative rounded-lg overflow-hidden shadow-lg">
                    <img src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Corporate Branding" 
                         class="w-full h-64 object-cover">
                    <div class="work-overlay absolute inset-0 bg-indigo-600 bg-opacity-90 flex flex-col justify-center items-center p-6 text-white">
                        <h3 class="text-xl font-bold mb-2">Corporate Branding</h3>
                        <p class="text-sm mb-4 text-center">Complete rebranding for a financial services company including stationery and marketing materials.</p>
                        <a href="#" class="border border-white px-4 py-2 rounded-full text-sm hover:bg-white hover:text-indigo-600 transition duration-300">
                            View Project
                        </a>
                    </div>
                </div>
                
                <!-- Project 5 -->
                <div class="work-item relative rounded-lg overflow-hidden shadow-lg">
                    <img src="https://images.unsplash.com/photo-1522542550221-31fd19575a2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Social Media Campaign" 
                         class="w-full h-64 object-cover">
                    <div class="work-overlay absolute inset-0 bg-indigo-600 bg-opacity-90 flex flex-col justify-center items-center p-6 text-white">
                        <h3 class="text-xl font-bold mb-2">Social Media Campaign</h3>
                        <p class="text-sm mb-4 text-center">Visual content creation for a 3-month social media campaign for a fashion brand.</p>
                        <a href="#" class="border border-white px-4 py-2 rounded-full text-sm hover:bg-white hover:text-indigo-600 transition duration-300">
                            View Project
                        </a>
                    </div>
                </div>
                
                <!-- Project 6 -->
                <div class="work-item relative rounded-lg overflow-hidden shadow-lg">
                    <img src="https://images.unsplash.com/photo-1581291518633-83b4ebd1d35e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Editorial Design" 
                         class="w-full h-64 object-cover">
                    <div class="work-overlay absolute inset-0 bg-indigo-600 bg-opacity-90 flex flex-col justify-center items-center p-6 text-white">
                        <h3 class="text-xl font-bold mb-2">Magazine Design</h3>
                        <p class="text-sm mb-4 text-center">Layout and art direction for a quarterly lifestyle magazine.</p>
                        <a href="#" class="border border-white px-4 py-2 rounded-full text-sm hover:bg-white hover:text-indigo-600 transition duration-300">
                            View Project
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="#" class="inline-flex items-center bg-indigo-600 text-white px-8 py-3 rounded-full font-medium hover:bg-indigo-700 transition-all duration-300 transform hover:-translate-y-1 shadow-lg hover:shadow-xl">
                    View All Projects <i class="fas fa-arrow-right ml-2"></i>
                </a>
            </div>
        </div>
    </section>
    
    <!-- Services Section -->
    <section id="services" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">My Services</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                    <div class="bg-indigo-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-pencil-alt text-indigo-600 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Brand Identity</h3>
                    <p class="text-gray-600 mb-4">
                        Crafting unique visual identities that capture your brand's essence and differentiate you in the market.
                    </p>
                    <ul class="text-gray-600 space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Logo Design
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Brand Guidelines
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Visual Systems
                        </li>
                    </ul>
                </div>
                
                <!-- Service 2 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                    <div class="bg-indigo-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-laptop text-indigo-600 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Digital Design</h3>
                    <p class="text-gray-600 mb-4">
                        Creating engaging digital experiences that captivate users and drive conversions.
                    </p>
                    <ul class="text-gray-600 space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> UI/UX Design
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Web Design
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Social Media Graphics
                        </li>
                    </ul>
                </div>
                
                <!-- Service 3 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                    <div class="bg-indigo-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-box-open text-indigo-600 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Packaging Design</h3>
                    <p class="text-gray-600 mb-4">
                        Designing packaging that stands out on shelves and creates memorable unboxing experiences.
                    </p>
                    <ul class="text-gray-600 space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Product Packaging
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Label Design
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Sustainable Solutions
                        </li>
                    </ul>
                </div>
                
                <!-- Service 4 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                    <div class="bg-indigo-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-newspaper text-indigo-600 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Print Design</h3>
                    <p class="text-gray-600 mb-4">
                        Creating impactful print materials that communicate your message effectively.
                    </p>
                    <ul class="text-gray-600 space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Business Cards
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Brochures
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Posters
                        </li>
                    </ul>
                </div>
                
                <!-- Service 5 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                    <div class="bg-indigo-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-bullhorn text-indigo-600 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Marketing Design</h3>
                    <p class="text-gray-600 mb-4">
                        Designing marketing materials that grab attention and drive engagement.
                    </p>
                    <ul class="text-gray-600 space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Advertising Campaigns
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Email Templates
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Promotional Materials
                        </li>
                    </ul>
                </div>
                
                <!-- Service 6 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-md hover:shadow-xl transition duration-300">
                    <div class="bg-indigo-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-paint-brush text-indigo-600 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Illustration</h3>
                    <p class="text-gray-600 mb-4">
                        Custom illustrations that bring your ideas to life with unique artistic style.
                    </p>
                    <ul class="text-gray-600 space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Digital Illustrations
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Character Design
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-indigo-600 mr-2"></i> Icon Sets
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Testimonials Section -->
    <section class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Client Testimonials</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-white p-8 rounded-lg shadow-md">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/43.jpg" alt="Sarah Johnson" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Sarah Johnson</h4>
                            <p class="text-sm text-gray-500">CEO, Nova Tech</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-4">
                        "Kamel transformed our brand identity completely. His designs captured our vision perfectly and helped us stand out in a crowded market. The attention to detail and strategic thinking behind his work is exceptional."
                    </p>
                    <div class="flex text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-white p-8 rounded-lg shadow-md">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael Chen" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Michael Chen</h4>
                            <p class="text-sm text-gray-500">Marketing Director, GreenLife</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-4">
                        "Working with Kamel on our packaging redesign was a game-changer. He understood our sustainability goals and created designs that were both beautiful and eco-conscious. Our sales increased by 30% after the redesign."
                    </p>
                    <div class="flex text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-white p-8 rounded-lg shadow-md">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/65.jpg" alt="Emma Rodriguez" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Emma Rodriguez</h4>
                            <p class="text-sm text-gray-500">Creative Director, Luxe Travel</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-4">
                        "Kamel's website design for our travel agency exceeded all expectations. He created an immersive digital experience that perfectly reflects our brand's luxury aesthetic. The user engagement metrics have been phenomenal."
                    </p>
                    <div class="flex text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star-half-alt"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Let's Work Together</h2>
                <div class="w-20 h-1 bg-indigo-600 mx-auto"></div>
            </div>
            
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-12 md:mb-0 md:pr-12">
                    <h3 class="text-2xl font-semibold mb-6">Get In Touch</h3>
                    <p class="text-gray-600 mb-8">
                        Have a project in mind or want to discuss potential collaboration? I'd love to hear from you. Fill out the form or reach out directly using the contact information below.
                    </p>
                    
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-envelope text-indigo-600"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold">Email</h4>
                                <p class="text-gray-600">hello@kamelrahmoun.com</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-phone-alt text-indigo-600"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold">Phone</h4>
                                <p class="text-gray-600">+1 (555) 123-4567</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-indigo-100 p-3 rounded-full mr-4">
                                <i class="fas fa-map-marker-alt text-indigo-600"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold">Studio</h4>
                                <p class="text-gray-600">123 Design Street, Creative City, CA 90210</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mt-8">
                        <h4 class="font-semibold mb-4">Follow Me</h4>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-gray-100 w-10 h-10 rounded-full flex items-center justify-center hover:bg-indigo-600 hover:text-white transition duration-300">
                                <i class="fab fa-behance"></i>
                            </a>
                            <a href="#" class="bg-gray-100 w-10 h-10 rounded-full flex items-center justify-center hover:bg-indigo-600 hover:text-white transition duration-300">
                                <i class="fab fa-dribbble"></i>
                            </a>
                            <a href="#" class="bg-gray-100 w-10 h-10 rounded-full flex items-center justify-center hover:bg-indigo-600 hover:text-white transition duration-300">
                                <i class="fab fa-instagram"></i>
                            </a>
                            <a href="#" class="bg-gray-100 w-10 h-10 rounded-full flex items-center justify-center hover:bg-indigo-600 hover:text-white transition duration-300">
                                <i class="fab fa-linkedin-in"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <form class="space-y-6">
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                            <div>
                                <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Name</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-600 focus:border-transparent">
                            </div>
                            <div>
                                <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-600 focus:border-transparent">
                            </div>
                        </div>
                        
                        <div>
                            <label for="subject" class="block text-sm font-medium text-gray-700 mb-1">Subject</label>
                            <input type="text" id="subject" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-600 focus:border-transparent">
                        </div>
                        
                        <div>
                            <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Message</label>
                            <textarea id="message" rows="5" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-600 focus:border-transparent"></textarea>
                        </div>
                        
                        <button type="submit" class="w-full bg-indigo-600 text-white px-6 py-3 rounded-lg font-medium hover:bg-indigo-700 transition duration-300">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <a href="#" class="text-2xl font-bold flex items-center">
                        <span class="text-indigo-400">KR</span>
                        <span class="ml-2">Kamel Rahmoun</span>
                    </a>
                    <p class="mt-2 text-gray-400">Creating visual stories that inspire and connect.</p>
                </div>
                
                <div class="flex flex-col items-center md:items-end">
                    <div class="flex space-x-6 mb-4">
                        <a href="#" class="hover:text-indigo-400 transition duration-300">
                            <i class="fab fa-behance"></i>
                        </a>
                        <a href="#" class="hover:text-indigo-400 transition duration-300">
                            <i class="fab fa-dribbble"></i>
                        </a>
                        <a href="#" class="hover:text-indigo-400 transition duration-300">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="hover:text-indigo-400 transition duration-300">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                    </div>
                    <p class="text-gray-400 text-sm">© 2023 Kamel Rahmoun. All rights reserved.</p>
                </div>
            </div>
        </div>
    </footer>
    
    <script>
        // Mobile menu toggle
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuBtn.addEventListener('click', () => {
            menuBtn.classList.toggle('active');
            mobileMenu.classList.toggle('open');
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                // Close mobile menu if open
                if (mobileMenu.classList.contains('open')) {
                    menuBtn.classList.remove('active');
                    mobileMenu.classList.remove('open');
                }
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Update active navigation link on scroll
        const sections = document.querySelectorAll('section');
        const navLinks = document.querySelectorAll('.nav-link');
        
        window.addEventListener('scroll', () => {
            let current = '';
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                
                if (pageYOffset >= (sectionTop - 100)) {
                    current = section.getAttribute('id');
                }
            });
            
            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === `#${current}`) {
                    link.classList.add('active');
                }
            });
        });
        
        // Work item hover effect
        const workItems = document.querySelectorAll('.work-item');
        
        workItems.forEach(item => {
            item.addEventListener('mouseenter', () => {
                const overlay = item.querySelector('.work-overlay');
                overlay.style.opacity = '1';
                overlay.style.transform = 'translateY(0)';
            });
            
            item.addEventListener('mouseleave', () => {
                const overlay = item.querySelector('.work-overlay');
                overlay.style.opacity = '0';
                overlay.style.transform = 'translateY(20px)';
            });
        });
    </script>
</body>
</html>
