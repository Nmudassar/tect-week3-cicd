## **multi-stage pipeline**

in Jenkins, where one job triggers another after it completes successfully. Let me break this down into a clear step-by-step process so you can replicate it.

---

## **Step 1: Configure First Job to Trigger a Second Job**

1. **Go to Jenkins Dashboard**.
2. **Click on the first job** (the one that runs the `uname` command).
3. Click **"Configure"**.
4. Scroll down to **Post-build Actions**.
5. Click **"Add post-build action" → "Build other projects"**.
6. Under **"Projects to build"**, type the name of the second job (the one that fetches the date).
7. **Avoid spaces or extra commas** – Jenkins may auto-add a comma, which can cause errors. Ensure it's just the job name.
8. **Select "Trigger only if build is stable"** (this ensures the second job only runs if the first one succeeds).
9. Click **"Save"**.

---

## **Step 2: Run and Observe the Jobs**

1. Go back to **Jenkins Dashboard**.
2. Click **"Build Now"** on the first job.
3. Go to **Jenkins Queue** to monitor the execution.
4. The first job should run, and immediately after completion, the second job should start.
5. Verify by checking:
   - **The first job’s Console Output** – it should show a successful execution.
   - **The second job’s Console Output** – it should mention being **"Started by upstream project first-job"**.

---

![First-project](<Screenshot 2025-02-05 115838.png>)

![get date/time](<Screenshot 2025-02-05 115913.png>)

## **Step 3: Troubleshooting**

If the second job does not run:

- Check **Post-build Actions** in the first job’s configuration.
- Make sure the job name is correct (no extra spaces or commas).
- Ensure the first job completes **successfully**.
- If necessary, check **Jenkins logs** for errors.

---

##
