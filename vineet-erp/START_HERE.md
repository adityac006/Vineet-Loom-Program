# START HERE — VINEET FURNISHINGS ERP

## What this package currently contains
- Professional responsive ERP interface
- Dashboard, Master Data, Loom Program, History and Analytics screens
- Loom numbers 1 to 52
- Supabase database schema with consistent BIGINT IDs
- GitHub/Vercel-ready project structure

## Important current status
This is the first build. The interface opens and can be deployed, but its forms currently use demonstration data inside the browser. The Supabase tables can be created now, but saving, login, import and shared live data require the next code connection.

## Simple setup process

### 1. Download and unzip
Unzip `vineet-furnishings-erp-starter.zip`. Open the folder named `vineet-erp`.

### 2. Create the Supabase database
1. Create/open a Supabase project.
2. Open SQL Editor.
3. Open `supabase/schema.sql` from this project.
4. Copy the complete SQL and run it once.
5. Confirm these tables appear: parties, beams, shades, sizes, designs, design_threads, loom_programs, loom_program_rows, production_entries.

### 3. Get Supabase connection values
In the Supabase project, open the Connect/API information and copy:
- Project URL
- Publishable/anon key

Keep these values private from screenshots and public messages.

### 4. Upload project to GitHub
1. Create/open one GitHub repository.
2. Upload the CONTENTS of the `vineet-erp` folder, not the zip file.
3. The repository root must show `package.json`, `index.html`, `src`, `supabase`, and `README.md`.
4. Commit the files.

### 5. Deploy through Vercel
1. Sign in to Vercel using GitHub.
2. Add New Project and import the GitHub repository.
3. Framework: Vite.
4. Build command: `npm run build`.
5. Output directory: `dist`.
6. Add environment variables:
   - `VITE_SUPABASE_URL`
   - `VITE_SUPABASE_ANON_KEY`
7. Deploy.

### 6. Open from mobile or computer
Vercel provides a website address. Open that address on a phone, tablet, laptop or desktop. The responsive interface will adjust to screen size.

## What is not connected in this first build
- Saving master data to Supabase
- Editing/deleting database records
- User login and roles
- Live production history
- Excel/PDF import
- PDF export
- Cloud synchronization between devices

These functions need application code connected to the Supabase tables. Running the SQL alone creates the database but does not connect the forms.
