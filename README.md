# MedWell

A small clinic back-office: doctors, patients, appointments and consultations.

The API is plain PHP — no framework. I wrote the routing, the controllers and the PDO
models by hand, which turned out to be the most useful part of the project. You don't
really appreciate what Django or Laravel do for you until you've done it yourself.

## What it does

- Keep records for doctors, each attached to a speciality
- Manage the patient register
- Book appointments between a patient and a doctor
- Record the consultation that follows
- Register and log in, with hashed passwords and a session per user

**Built with** PHP 8, PDO, React 19, Vite, Bootstrap and MySQL.

## Running it

You'll need XAMPP (or WAMP) and Node 18+.

The front end calls `http://localhost/Clinique/Backend`, so the project has to sit in
your web root under the name `Clinique`:

```bash
git clone https://github.com/salmenhammami/MedWell.git
# copy it into C:\xampp\htdocs\Clinique  (or /var/www/html/Clinique)
```

Create a MySQL database called `clinique` and import `database/schema.sql`. Then
start Apache and MySQL, and run the front end:

```bash
cd Frontend
npm install && npm run dev
```

If you'd rather serve the API somewhere else, change `API_URL` in `Frontend/src/api.js`.

## Honest notes

A coursework project, not something to deploy. The database credentials are hard-coded,
CORS is wide open alongside cookie sessions, and roles are stored on login but not yet
checked on every endpoint.

---

**Salmen Hammami** · [GitHub](https://github.com/salmenhammami) · [LinkedIn](https://www.linkedin.com/in/salmenhammami/)
