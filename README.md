- 👋 Hi, I’m @Nightovvl
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Nightovvl/Nightovvl is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->https://sharetext.me/f1valx9zhm
var gr = new GlideRecord('sys_user');
gr.addEncodedQuery();//query to find out user records to update
gr.query();
while (gr.next()) {
   
      gr.time_zone = 'Canada/Pacific'; // you can get these values from sys_choice table for time_zone field like https://<<<your_instance_name>>>.service-now.com/sys_choice_list.do?sysparm_query=element%3Dtime_zone%5Ename%3Dsys_user&sysparm_view=
      gr.setWorkflow(false); // Don't run business rules for this update
      gr.update();
   
}
