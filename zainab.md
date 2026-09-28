open your Next.js project in vs code.
open terminal.
i can run this code.
.npm run dev
then open in google.
.http://localhost:3000.
.we connected Next.js to supabase using the CMD/terminal,
and then used supabase to connect our database with the Next.js project.
Supabase is an online database platform.
step :1
Create a supabase project.
Create a database table in Supabase.
Create or open your Next.js project.
Install the Supabase package.
It is used to store and manage data.
import { createClient } from '@supabase/supabase-js';

const supabase = createClient(
  process.env.NEXT_PUBLIC_SUPABASE_URL,
  process.env.NEXT_PUBLIC_SUPABASE_ANON_KEY
);

export default function Home() {
  return (
    <main>
      <h1>Supabase</h1>
      <p>Supabase is an online database platform.</p>
    </main>
  );
}
step :2
Next.js is used to build the website/frontend.
export default function Home() {
  return (
    <main>
      <h1>My Website</h1>
      <p>Next.js is used to build the website/frontend.</p>
    </main>
  );
}
Next.js is used to build websites.
It is a React framework.
It helps create the frontend.
It can connect with databases like Supabase.
It helps build fast web applications.
step :3
Supabase and Next.js can be connected to send and receive data.
import { supabase } from "@/lib/supabase";

export default async function Home() {
  const { data } = await supabase.from("department").select("*");

  return <div>{JSON.stringify(data)}</div>;
}
Create a Supabase project and database table.
Create or open your Next.js project.
Send, receive, and display data between Next.js and Supabase.
Data can be inserted into Supabase from a Next.js form.
step :4
Data can be displayed on the Next.js frontend.
import { supabase } from "@/lib/supabase";

export default async function Home() {
  const { data } = await supabase.from("department").select("*");

  return <div>{JSON.stringify(data)}</div>;
}
Create a database table in Supabase.
Add some data to the table.
Connect Supabase with Next.js.
Create a Supabase client.
Fetch the data from Supabase.
Store the fetched data in Next.js.
Display the data on the webpage.
The user can now see the Supabase data on the frontend.
step :5
can also be updated and deleted.
import { supabase } from "@/lib/supabase";

export default async function Home() {
  const { data } = await supabase.from("department").select("*");

  return <div>{JSON.stringify(data)}</div>;
}
Connect Supabase with Next.js.
Select the data you want to change.
Update the existing data when needed.
Select the data you want to remove.
Delete the unwanted data.
The changes are saved in the Supabase database.







