<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced HTML5 Elements and Forms</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
            color: #333;
        }
        header, main, footer {
            max-width: 1000px;
            margin: 0 auto;
        }
        h1, h2 {
            color: #2c3e50;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            margin: 20px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        th, td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        th {
            background-color: #f2f2f2;
        }
        form {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }
        input[type="radio"], input[type="checkbox"] {
            width: auto;
            margin-right: 10px;
        }
        button {
            background-color: #3498db;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #2980b9;
        }
        section {
            margin: 30px 0;
        }
    </style>
</head>
<body>
    <!-- Main header section -->
    <header>
        <h1>Advanced HTML5 Elements and Forms</h1>
    </header>

    <main>
        <!-- Section 1: Ordered List with Roman Numerals -->
        <section id="list-section">
            <h2>Web Development Fundamentals</h2>
            <p>The following are essential technologies for modern web development:</p>
            <ol type="I">
                <li>HTML5 - Structure and semantics</li>
                <li>CSS3 - Styling and layout</li>
                <li>JavaScript - Interactivity and functionality</li>
                <li>Responsive Design - Mobile compatibility</li>
                <li>Accessibility - Inclusive user experience</li>
            </ol>
        </section>

        <!-- Section 2: External Image from Pexels -->
        <section id="image-section">
            <h2>Web Development Workspace</h2>
            <img src="https://images.pexels.com/photos/574071/pexels-photo-574071.jpeg" 
                 alt="Laptop with code on the screen on a desk with coffee" 
                 width="800" height="533">
            <p>A typical developer workspace with code and coffee.</p>
        </section>

        <!-- Section 3: Table of Contacts -->
        <section id="table-section">
            <h2>Contact Directory</h2>
            <table>
                <thead>
                    <tr>
                        <th>Name</th>
                        <th>Address</th>
                        <th>Mobile</th>
                        <th>Email</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>John Smith</td>
                        <td>123 Main St, New York, NY</td>
                        <td>(555) 123-4567</td>
                        <td>john.smith@example.com</td>
                    </tr>
                    <tr>
                        <td>Emma Johnson</td>
                        <td>456 Oak Ave, Chicago, IL</td>
                        <td>(555) 234-5678</td>
                        <td>emma.j@example.com</td>
                    </tr>
                    <tr>
                        <td>Michael Brown</td>
                        <td>789 Pine Rd, San Francisco, CA</td>
                        <td>(555) 345-6789</td>
                        <td>mbrown@example.com</td>
                    </tr>
                    <tr>
                        <td>Olivia Davis</td>
                        <td>101 Maple Dr, Austin, TX</td>
                        <td>(555) 456-7890</td>
                        <td>olivia.d@example.com</td>
                    </tr>
                    <tr>
                        <td>William Wilson</td>
                        <td>202 Cedar Ln, Seattle, WA</td>
                        <td>(555) 567-8901</td>
                        <td>will.wilson@example.com</td>
                    </tr>
                </tbody>
            </table>
        </section>

        <!-- Section 4: Registration Form -->
        <section id="form-section">
            <h2>Registration Form</h2>
            <form id="registration-form" action="#" method="post">
                <!-- Personal Information -->
                <fieldset>
                    <legend>Personal Information</legend>
                    
                    <div class="form-group">
                        <label for="fullname">Full Name:</label>
                        <input type="text" id="fullname" name="fullname" placeholder="Enter your full name" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="email">Email Address:</label>
                        <input type="email" id="email" name="email" placeholder="your.email@example.com" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="password">Password:</label>
                        <input type="password" id="password" name="password" minlength="8" 
                               placeholder="Minimum 8 characters" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="birthdate">Date of Birth:</label>
                        <input type="date" id="birthdate" name="birthdate" required>
                    </div>
                </fieldset>
                
                <!-- Preferences -->
                <fieldset>
                    <legend>Preferences</legend>
                    
                    <div class="form-group">
                        <label for="occupation">Occupation:</label>
                        <select id="occupation" name="occupation" required>
                            <option value="">-- Select your occupation --</option>
                            <option value="student">Student</option>
                            <option value="developer">Web Developer</option>
                            <option value="designer">Designer</option>
                            <option value="manager">Project Manager</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <p><strong>Experience Level:</strong></p>
                        <input type="radio" id="beginner" name="experience" value="beginner" required>
                        <label for="beginner">Beginner</label><br>
                        
                        <input type="radio" id="intermediate" name="experience" value="intermediate">
                        <label for="intermediate">Intermediate</label><br>
                        
                        <input type="radio" id="advanced" name="experience" value="advanced">
                        <label for="advanced">Advanced</label>
                    </div>
                    
                    <div class="form-group">
                        <p><strong>Areas of Interest:</strong></p>
                        <input type="checkbox" id="html" name="interests" value="html">
                        <label for="html">HTML5</label><br>
                        
                        <input type="checkbox" id="css" name="interests" value="css">
                        <label for="css">CSS3</label><br>
                        
                        <input type="checkbox" id="javascript" name="interests" value="javascript">
                        <label for="javascript">JavaScript</label><br>
                        
                        <input type="checkbox" id="responsive" name="interests" value="responsive">
                        <label for="responsive">Responsive Design</label>
                    </div>
                </fieldset>
                
                <!-- Additional Information -->
                <fieldset>
                    <legend>Additional Information</legend>
                    
                    <div class="form-group">
                        <label for="comments">Comments or Questions:</label>
                        <textarea id="comments" name="comments" rows="4" placeholder="Share your thoughts..."></textarea>
                    </div>
                    
                    <div class="form-group">
                        <input type="checkbox" id="terms" name="terms" required>
                        <label for="terms">I agree to the Terms and Conditions</label>
                    </div>
                </fieldset>
                
                <button type="submit">Register</button>
                <button type="reset">Clear Form</button>
            </form>
        </section>

        <!-- Section 5: Multimedia Elements -->
        <section id="multimedia-section">
            <h2>Multimedia Elements</h2>
            
            <!-- Audio Element -->
            <h3>Audio Sample</h3>
            <audio controls>
                <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
                Your browser does not support the audio element.
            </audio>
            
            <!-- Video Element -->
            <h3>Video Sample</h3>
            <video width="640" height="360" controls>
                <source src="https://samplelib.com/lib/preview/mp4/sample-5s.mp4" type="video/mp4">
                Your browser does not support the video element.
            </video>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Advanced HTML5 Demo | Created for educational purposes</p>
    </footer>
</body>
</html>
