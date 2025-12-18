<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ධනා Free+Fire - Professional Website</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Base Styles and WhatsApp-inspired Color Theme */
        :root {
             --whatsapp-green: #2E7D32;           /* Deep emerald green */
--whatsapp-green-dark: #1B5E20;
--whatsapp-green-light: #E8F5E9;
--bg-primary: #000000;               /* Pure black canvas */
--accent-blue: #00D4FF;              /* Electric cyan accent */
--ui-surface: #1A1A1A;               /* UI containers */
--ui-elevated: #2A2A2A;              /* Elevated surfaces */
--text-primary: #FFFFFF;             /* Primary text */
--text-secondary: #AAAAAA;           /* Secondary text */
--accent-orange: #FF6B35;            /* Call-to-action */
--status-success: #00D95F;           /* Success states */
--status-danger: #FF375F;            /* Error/danger */
--border-subtle: rgba(255,255,255,0.1); /* Subtle borders */
--border-strong: rgba(255,255,255,0.2); /* Strong borders */
--overlay-hover: rgba(255,255,255,0.05); /* Hover states */
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--whatsapp-light-gray);
            color: var(--text-dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header and Logo */
        header {
            background-color: var(--whatsapp-green);
            padding: 15px 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .logo-container {
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .logo {
            font-size: 2.8rem;
            font-weight: bold;
            color: var(--white);
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
            padding: 10px;
            border-radius: 8px;
            background-color: rgba(255, 255, 255, 0.1);
        }
        
        /* Navigation Tabs */
        .tabs {
            display: flex;
            background-color: var(--white);
            border-bottom: 1px solid var(--border-color);
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
        }
        
        .tab {
            flex: 1;
            text-align: center;
            padding: 18px 10px;
            font-size: 1.1rem;
            font-weight: 600;
            color: var(--text-light);
            cursor: pointer;
            transition: all 0.3s ease;
            border-bottom: 3px solid transparent;
        }
        
        .tab:hover {
            background-color: var(--whatsapp-gray);
            color: var(--whatsapp-green);
        }
        
        .tab.active {
            color: var(--whatsapp-green);
            border-bottom: 3px solid var(--whatsapp-green);
            background-color: rgba(18, 140, 126, 0.05);
        }
        
        /* Tab Content */
        .tab-content {
            display: none;
            padding: 30px 20px;
            animation: fadeIn 0.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .tab-content.active {
            display: block;
        }
        
        /* Home Tab Styles */
        .contact-section {
            background-color: var(--white);
            border-radius: 12px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            max-width: 800px;
            margin: 0 auto;
        }
        
        .contact-title {
            color: var(--whatsapp-green);
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 1px solid var(--border-color);
            font-size: 1.8rem;
        }
        
        .contact-field {
            margin-bottom: 25px;
            padding: 15px;
            border-radius: 8px;
            background-color: var(--whatsapp-light-gray);
            border-left: 4px solid var(--whatsapp-light-green);
        }
        
        .contact-field i {
            color: var(--whatsapp-green);
            margin-right: 12px;
            font-size: 1.2rem;
            width: 30px;
        }
        
        .field-label {
            font-weight: 600;
            color: var(--text-dark);
            margin-bottom: 5px;
            display: block;
        }
        
        .field-value {
            color: var(--text-light);
            font-size: 1.1rem;
        }
        
        /* Files Tab Styles */
        .files-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 20px;
        }
        
        .file-card {
            background-color: var(--white);
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 1px solid var(--border-color);
        }
        
        .file-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        .card-image {
            height: 180px;
            width: 100%;
            background-color: var(--whatsapp-gray);
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }
        
        .card-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .file-card:hover .card-image img {
            transform: scale(1.05);
        }
        
        .round-icon {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background-color: var(--whatsapp-light-green);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2.5rem;
        }
        
        .card-content {
            padding: 20px;
        }
        
        .card-title {
            color: var(--whatsapp-green);
            margin-bottom: 10px;
            font-weight: 600;
            font-size: 1.2rem;
        }
        
        .card-description {
            color: var(--text-light);
            margin-bottom: 20px;
            height: 60px;
            overflow: hidden;
            font-size: 0.95rem;
        }
        
        .card-link {
            display: inline-block;
            background-color: var(--whatsapp-green);
            color: white;
            padding: 10px 20px;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.3s ease;
        }
        
        .card-link:hover {
            background-color: var(--whatsapp-light-green);
        }
        
        .download-info {
            font-size: 0.85rem;
            color: var(--text-light);
            margin-top: 8px;
            font-style: italic;
        }
        
        /* About Tab Styles */
        .about-section {
            background-color: var(--white);
            border-radius: 12px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            max-width: 800px;
            margin: 0 auto;
        }
        
        .about-title {
            color: var(--whatsapp-green);
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 1px solid var(--border-color);
            font-size: 1.8rem;
        }
        
        .poem-container {
            background-color: var(--whatsapp-chat-green);
            border-radius: 10px;
            padding: 25px;
            margin-top: 20px;
            border-left: 5px solid var(--whatsapp-green);
            font-size: 1.2rem;
            line-height: 1.8;
            text-align: center;
        }
        
        .poem-line {
            margin-bottom: 15px;
        }
        
        .poem-author {
            margin-top: 20px;
            font-style: italic;
            color: var(--text-light);
        }
        
        /* Editable Field Indicators */
        .editable-indicator {
            display: inline-block;
            background-color: rgba(37, 211, 102, 0.1);
            color: var(--whatsapp-light-green);
            font-size: 0.8rem;
            padding: 3px 8px;
            border-radius: 4px;
            margin-left: 10px;
            vertical-align: middle;
        }
        
        .upload-guide {
            background-color: rgba(18, 140, 126, 0.05);
            border: 1px dashed var(--whatsapp-green);
            border-radius: 8px;
            padding: 15px;
            margin-top: 10px;
            font-size: 0.9rem;
            color: var(--text-light);
        }
        
        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            margin-top: 40px;
            color: var(--text-light);
            border-top: 1px solid var(--border-color);
            font-size: 0.9rem;
        }
        
        /* Responsive Styles */
        @media (max-width: 768px) {
            .logo {
                font-size: 2.2rem;
            }
            
            .tab {
                padding: 15px 5px;
                font-size: 1rem;
            }
            
            .files-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
                gap: 20px;
            }
            
            .contact-section, .about-section {
                padding: 20px;
            }
            
            .poem-container {
                padding: 20px;
                font-size: 1.1rem;
            }
        }
        
        @media (max-width: 480px) {
            .logo {
                font-size: 1.8rem;
            }
            
            .tabs {
                flex-direction: column;
            }
            
            .tab {
                padding: 12px;
                border-bottom: 1px solid var(--border-color);
                border-left: 4px solid transparent;
            }
            
            .tab.active {
                border-left: 4px solid var(--whatsapp-green);
                border-bottom: 1px solid var(--border-color);
            }
            
            .files-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header with Sinhala Logo -->
    <header>
        <div class="container">
            <div class="logo-container">
                <div class="logo">DHANA FREEFIRE</div>
            </div>
        </div>
    </header>
    
    <!-- Navigation Tabs -->
    <div class="tabs container">
        <div class="tab active" data-tab="home">Home</div>
        <div class="tab" data-tab="files">Files</div>
        <div class="tab" data-tab="about">About</div>
    </div>
    
    <!-- Main Content Area -->
    <main class="container">
        <!-- Home Tab Content -->
        <section id="home" class="tab-content active">
            <h2 class="contact-title">Contact Details <span class="editable-indicator">Editable Section</span></h2>
            
            <div class="contact-section">
                <!-- Update phone number here -->
                <div class="contact-field">
                    <i class="fas fa-phone-alt"></i>
                    <div class="field-label">Phone Number</div>
                    <div class="field-value">+94 77 123 4567</div>
                    <div class="editable-indicator">Update phone number here</div>
                </div>
                
                <!-- Update email here -->
                <div class="contact-field">
                    <i class="fas fa-envelope"></i>
                    <div class="field-label">Email Address</div>
                    <div class="field-value">contact@dhanafreefire.lk</div>
                    <div class="editable-indicator">Update email here</div>
                </div>
                
                <!-- Update logo here -->
                <div class="contact-field">
                    <i class="fas fa-image"></i>
                    <div class="field-label">Logo Image</div>
                    <div class="field-value">Current logo: "ධනා Free+Fire" in Sinhala script</div>
                    <div class="editable-indicator">Update logo here</div>
                </div>
                
                <div class="contact-field">
                    <i class="fas fa-info-circle"></i>
                    <div class="field-label">Instructions</div>
                    <div class="field-value">To update any information, simply edit the HTML content in the sections marked with the green "Editable Section" indicator.</div>
                </div>
            </div>
        </section>
        
        <!-- Files Tab Content -->
        <section id="files" class="tab-content">
            <h2 class="contact-title">File Collection <span class="editable-indicator">12 Card Slots</span></h2>
            
            <div class="upload-guide">
                <strong>How to upload images:</strong> Replace the image URL in the "src" attribute of each img tag with your own image URL or local file path. For download links, update the "href" attribute in the a tag with your actual file URL.
            </div>
            
            <div class="files-grid">
                <!-- 
                FIRST SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://raw.githubusercontent.com/jackblasterfuze-commits/DANA-45/refs/heads/main/6.jpeg" alt="Food Image">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Healthy Recipes</div>
                        <div class="card-description">
                            Collection of healthy and delicious recipes for everyday meals. Includes vegetarian and vegan options.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://drive.google.com/file/d/1-Cfa79dpSzu32l46Y8aEIqWpdOtt_uPS/view?usp=drivesdk" class="card-link" download>Download File</a>
                        <div class="download-info">PDF format, 2.4 MB</div>
                        <div class="editable-indicator">First slot</div>
                    </div>
                </div>
                
                <!-- 
                SECOND SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://raw.githubusercontent.com/jackblasterfuze-commits/DANA-45/refs/heads/main/1.jpeg" alt="Technology Image">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Tech Guide 2023</div>
                        <div class="card-description">
                            Comprehensive guide to the latest technology trends and innovations in 2023.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://drive.google.com/file/d/10BXV0rRV47V0VV1_U-yOIw3dUSXaTIVb/view?usp=drivesdk" class="card-link" download>Download File</a>
                        <div class="download-info">PDF format, 5.1 MB</div>
                        <div class="editable-indicator">Second slot</div>
                    </div>
                </div>
                
                <!-- 
                THIRD SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1477346611705-65d1883cee1e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Mountain Landscape">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Travel Photography</div>
                        <div class="card-description">
                            Beautiful collection of travel photography from around the world. High resolution images.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/travel-photos.zip" class="card-link" download>Download File</a>
                        <div class="download-info">ZIP format, 18.7 MB</div>
                        <div class="editable-indicator">Third slot</div>
                    </div>
                </div>
                
                <!-- 
                FOURTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1558618666-fcd25c85cd64?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Business Meeting">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Business Strategy</div>
                        <div class="card-description">
                            Effective business strategies for startups and established companies. Includes case studies.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/business-strategy.docx" class="card-link" download>Download File</a>
                        <div class="download-info">DOCX format, 3.2 MB</div>
                        <div class="editable-indicator">Fourth slot</div>
                    </div>
                </div>
                
                <!-- 
                FIFTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1542744095-fcf48d80b0fd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Fitness Workout">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Fitness Program</div>
                        <div class="card-description">
                            12-week fitness program with workout routines, nutrition guides, and progress tracking.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/fitness-program.pdf" class="card-link" download>Download File</a>
                        <div class="download-info">PDF format, 4.5 MB</div>
                        <div class="editable-indicator">Fifth slot</div>
                    </div>
                </div>
                
                <!-- 
                SIXTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1559136555-9303baea8ebd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Cooking Ingredients">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Cooking Basics</div>
                        <div class="card-description">
                            Essential cooking techniques and recipes for beginners. Step-by-step instructions with images.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/cooking-basics.pdf" class="card-link" download>Download File</a>
                        <div class="download-info">PDF format, 6.3 MB</div>
                        <div class="editable-indicator">Sixth slot</div>
                    </div>
                </div>
                
                <!-- 
                SEVENTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Team Collaboration">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Team Management</div>
                        <div class="card-description">
                            Guide to effective team management, collaboration tools, and productivity techniques.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/team-management.pptx" class="card-link" download>Download File</a>
                        <div class="download-info">PPTX format, 8.9 MB</div>
                        <div class="editable-indicator">Seventh slot</div>
                    </div>
                </div>
                
                <!-- 
                EIGHTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1556761175-b413da4baf72?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Office Workspace">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Productivity Tools</div>
                        <div class="card-description">
                            Collection of productivity tools, apps, and techniques to optimize your workday.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/productivity-tools.zip" class="card-link" download>Download File</a>
                        <div class="download-info">ZIP format, 12.1 MB</div>
                        <div class="editable-indicator">Eighth slot</div>
                    </div>
                </div>
                
                <!-- 
                NINTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1551434678-e076c223a692?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Programming Code">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Coding Tutorials</div>
                        <div class="card-description">
                            Beginner to advanced coding tutorials in Python, JavaScript, and other popular languages.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/coding-tutorials.zip" class="card-link" download>Download File</a>
                        <div class="download-info">ZIP format, 15.8 MB</div>
                        <div class="editable-indicator">Ninth slot</div>
                    </div>
                </div>
                
                <!-- 
                TENTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Study Materials">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Study Materials</div>
                        <div class="card-description">
                            Comprehensive study materials for various subjects. Perfect for students and lifelong learners.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/study-materials.pdf" class="card-link" download>Download File</a>
                        <div class="download-info">PDF format, 7.6 MB</div>
                        <div class="editable-indicator">Tenth slot</div>
                    </div>
                </div>
                
                <!-- 
                ELEVENTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1532094349884-543bc11b234d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Creative Design">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Design Resources</div>
                        <div class="card-description">
                            Collection of design resources including templates, icons, fonts, and color palettes.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/design-resources.zip" class="card-link" download>Download File</a>
                        <div class="download-info">ZIP format, 22.3 MB</div>
                        <div class="editable-indicator">Eleventh slot</div>
                    </div>
                </div>
                
                <!-- 
                TWELFTH SLOT: 
                1. To upload photo: Replace the src attribute in img tag with your image URL
                2. Update description text
                3. Update download link in href attribute
                -->
                <div class="file-card">
                    <div class="card-image">
                        <!-- REPLACE THIS IMAGE URL WITH YOUR OWN IMAGE -->
                        <img src="https://images.unsplash.com/photo-1563013544-824ae1b704d3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="Finance Chart">
                    </div>
                    <div class="card-content">
                        <div class="card-title">Financial Planning</div>
                        <div class="card-description">
                            Guide to personal financial planning, budgeting, investing, and wealth management.
                        </div>
                        <!-- UPDATE DOWNLOAD LINK HERE: Replace href with your actual file URL -->
                        <a href="https://example.com/files/financial-planning.xlsx" class="card-link" download>Download File</a>
                        <div class="download-info">XLSX format, 3.8 MB</div>
                        <div class="editable-indicator">Twelfth slot</div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- About Tab Content -->
        <section id="about" class="tab-content">
            <h2 class="contact-title">About Us <span class="editable-indicator">Editable Content</span></h2>
            
            <div class="about-section">
                <p>Welcome to <strong>DANA Free+Fire</strong>, a professional platform dedicated to providing quality resources and information.</p>
                
                567
                <p>*🔴 මේ වගේ සුපිරි ම LOGOS, YT THIMBNAILS, DIAMOND STORE POSTS පොඩි මුදලකට හදලා දෙනවා🔴* 

 *🔴100%ක් විශ්වාසවන්තව අප සමග කටයුතු කරන්න.🔴* 


 *👉2d logo price - RS.50* 
 *👉Normal logo price - RS.90* 
 *👉Diamond store post price - RS.120* 
 *👉YT thimbnail price - dialog data card* 


 *🔴 මේ වගේ දේවල් හදන්නත් කියලා දෙනවා<br>
  පොඩි Price එකකට.* 

 *👉 හදන්න කියලා දෙනවට අය කරන්නේ රු.200ක් පමණි 👈* 

 🪀*WP NUM - 0741048179*</p>
                
                
                <div class="editable-indicator" style="margin-top: 20px;">ERROR 404 </div>
            </div>
        </section>
    </main>
    
    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2023 ධනා Free+Fire. All rights reserved.</p>
            <p>Professional Website | Designed for easy content management</p>
        </div>
    </footer>
    
    <script>
        // Tab switching functionality
        document.addEventListener('DOMContentLoaded', function() {
            const tabs = document.querySelectorAll('.tab');
            const tabContents = document.querySelectorAll('.tab-content');
            
            tabs.forEach(tab => {
                tab.addEventListener('click', () => {
                    // Remove active class from all tabs and contents
                    tabs.forEach(t => t.classList.remove('active'));
                    tabContents.forEach(content => content.classList.remove('active'));
                    
                    // Add active class to clicked tab
                    tab.classList.add('active');
                    
                    // Show corresponding content
                    const tabId = tab.getAttribute('data-tab');
                    document.getElementById(tabId).classList.add('active');
                });
            });
            
            // Handle download tracking (for demonstration)
            const downloadLinks = document.querySelectorAll('.card-link');
            downloadLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    // In a real implementation, you might want to track downloads here
                    console.log('Download initiated: ' + this.getAttribute('href'));
                    
                    // For demo purposes, if the link points to example.com, show an alert
                    if (this.getAttribute('href').includes('example.com')) {
                        e.preventDefault();
                        alert('This is a demo link. In the actual website, replace this with your actual file URL.');
                    }
                });
            });
        });
    </script>
</body>
</html>
