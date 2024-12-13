# Patient-Doctor-App
made in html (demo)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Healthcare Management System</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f0f0f0;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        .form-section {
            margin-bottom: 30px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input[type="text"],
        input[type="email"],
        input[type="tel"],
        input[type="date"],
        textarea,
        select {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
        h2 {
            color: #333;
            border-bottom: 2px solid #4CAF50;
            padding-bottom: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Healthcare Management System</h1>

        <!-- Doctor Registration Form -->
        <div class="form-section">
            <h2>Doctor Registration</h2>
            <form id="doctorForm">
                <div class="form-group">
                    <label for="doctorName">Full Name:</label>
                    <input type="text" id="doctorName" name="doctorName" required>
                </div>
                <div class="form-group">
                    <label for="specialization">Specialization:</label>
                    <input type="text" id="specialization" name="specialization" required>
                </div>
                <div class="form-group">
                    <label for="doctorEmail">Email:</label>
                    <input type="email" id="doctorEmail" name="doctorEmail" required>
                </div>
                <div class="form-group">
                    <label for="doctorPhone">Phone:</label>
                    <input type="tel" id="doctorPhone" name="doctorPhone" required>
                </div>
                <div class="form-group">
                    <label for="doctorLicense">License Number:</label>
                    <input type="text" id="doctorLicense" name="doctorLicense" required>
                </div>
                <button type="submit">Register Doctor</button>
            </form>
        </div>

        <!-- Patient Registration Form -->
        <div class="form-section">
            <h2>Patient Registration</h2>
            <form id="patientForm">
                <div class="form-group">
                    <label for="patientName">Full Name:</label>
                    <input type="text" id="patientName" name="patientName" required>
                </div>
                <div class="form-group">
                    <label for="patientDOB">Date of Birth:</label>
                    <input type="date" id="patientDOB" name="patientDOB" required>
                </div>
                <div class="form-group">
                    <label for="patientEmail">Email:</label>
                    <input type="email" id="patientEmail" name="patientEmail" required>
                </div>
                <div class="form-group">
                    <label for="patientPhone">Phone:</label>
                    <input type="tel" id="patientPhone" name="patientPhone" required>
                </div>
                <div class="form-group">
                    <label for="medicalHistory">Medical History:</label>
                    <textarea id="medicalHistory" name="medicalHistory" rows="4"></textarea>
                </div>
                <div class="form-group">
                    <label for="currentMedications">Current Medications:</label>
                    <textarea id="currentMedications" name="currentMedications" rows="4"></textarea>
                </div>
                <div class="form-group">
                    <label for="assignedDoctor">Assigned Doctor:</label>
                    <select id="assignedDoctor" name="assignedDoctor" required>
                        <option value="">Select a doctor</option>
                        <option value="doc1">Dr. Smith</option>
                        <option value="doc2">Dr. Johnson</option>
                        <option value="doc3">Dr. Williams</option>
                    </select>
                </div>
                <button type="submit">Register Patient</button>
            </form>
        </div>
    </div>

    <script>
        // Basic form submission handling
        document.getElementById('doctorForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Doctor registration submitted!');
            // Here you would typically send the data to a server
        });

        document.getElementById('patientForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Patient registration submitted!');
            // Here you would typically send the data to a server
        });
    </script>
</body>
</html>
