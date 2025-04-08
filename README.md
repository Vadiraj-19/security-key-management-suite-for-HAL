# security-key-management-suite-for-HAL


## 1. User Roles & Access Control
      Implement Role-Based Access Control (RBAC):

       1.Admin (Department Authority): Can add/edit personnel for their department only.
       2.Security: Can issue/return keys by entering PB number.
       3.Auditor: Can only view logs and reports (read-only access).

## 2. Department-Wise Assignment
      1.Each department can assign multiple authorized persons using their PB numbers.
      2.Only department-specific admins can manage their personnel.
      3.Prevent cross-department access.

## 3. PB Number Validation
      When someone requests a key at the security counter:
      1.Security enters the PB number.
      2.System checks if PB number is active and assigned.
      3.If valid → show name, department, photo, and proceed to issue the key.

## 4. Add/Edit/Delete Authorized Personnel
      Add personnel by entering:
      1.Name
      2.PB Number
      3.Department
      4.Upload Photo
      5.Valid Until Date
      6.Edit existing records if updates are needed.
      7.Delete record when the person retires or is no longer eligible.

## 5. Key Issue & Return Tracking
      1.Store key issue time, PB number, department, name.
      2.When returned, update the return time and status.
      3.Highlight keys that are not returned after a set duration.

## 6. Key Status Dashboard
      Visual display of:
      1.Total Keys
      2.Keys Issued (Active)
      3.Keys Returned
      4.Overdue Keys
      5.Filter by department, PB number, date range.

## 7. Photo ID Verification
      1.Display uploaded photo of personnel during PB number verification at security.
      2.Ensures visual confirmation of identity.

## 8. Access Expiry
      1.Set an expiry date for access (e.g., 31st Dec 2025).
      2.System auto-disables personnel after this date.
      3.Alert admin one week before access expiry.

## 9. Downloadable Reports (Excel or PDF)
      Allow authorized users to download key logs based on:
      1.Department
      2.PB number
      3.Date range
      4.Helps in audit and official reporting.

#HAL Key Management System – Full Project Blueprint
## 1. Tech Stack Overview
            Part	             Tech
            Frontend	 React.js + Tailwind CSS
            Backend	 Node.js + Express.js
            Database	 MongoDB (Mongoose)
            Auth	        JWT + bcrypt
            File Upload	 Multer / Cloudinary
            Deployment	 Vercel (frontend), Render (backend), MongoDB Atlas (DB)
