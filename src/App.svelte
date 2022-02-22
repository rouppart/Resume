<script lang="ts">
	import Tailwind from './Tailwind.svelte';
	import Posting from './components/Posting.svelte';
</script>

<Tailwind />

<main class="bg-white mx-auto">

	<div class="my-4 ml-6">
		<h1 class="text-4xl font-bold tracking-widest">Robert Trad</h1>
		<h2 class="text-xl text-gray-500">Software Developer</h2>
	</div>

	<div class="col-span-2 mt-auto mb-4 mr-6">
		Intermediate software developer with a wide-ranging skill set acquired over 9 years of IT management and support,
		looking to move to a more development focused career.
	</div>

	<div class="col-span-3 flex justify-around items-center bg-gray-200 py-3">
		<span><em class="fas fa-passport fa-lg"></em> Lebanese, Canadian</span>
		<span><em class="fas fa-home fa-lg"></em> Beirut, Lebanon</span>
		<span><em class="fas fa-phone-alt fa-lg"></em> <a href="tel:+9613953017">+961 3 953 017</a></span>
		<span><em class="fas fa-envelope fa-lg"></em> <a href="mailto: roberttrad@gmail.com" target="_blank">roberttrad@gmail.com</a></span>
		<span><em class="fab fa-linkedin fa-lg"></em> <a href="https://www.linkedin.com/in/robert-trad" target="_blank">robert-trad</a></span>
		<span><em class="fab fa-github fa-lg"></em> <a href="https://github.com/rouppart" target="_blank">rouppart</a></span>
	</div>

	<div class="flex flex-col space-y-6 m-3">

		<div class="section"><span>Professional Experience</span></div>

		<Posting position="IT Manager" organization="Saad & Trad SAL" location="Beirut, Lebanon" startDate="2012-08" endDate="Present">
			<ul>
				<li>
					In charge of implementing an automotive ERP called Incadea, based on <i>Microsoft Dynamics NAV</i> since 2012.
					Reduced cost of consulting, increased quality and speed of deliverables by learning <i>C/AL</i>, Incadea's development language.
					Migrated data between systems using <i>Pandas</i>.
				</li>
				<li>
					Currently writing a new ERP from scratch based on a Microservice architecture using <i>Svelte</i> and <i>Tailwind</i> for the frontend,
					and <i>GraphQL</i> implemented with <i>Starlette</i> in <i>Python</i> for the backend with <i>Postgresql</i> as a database and <i>SQLAlchemy</i> as an ORM.
					Every pair of frontend/backend represents a department.
				</li>
				<li>
					Trained all users from all departments on how to use the new software.
					Capitalized on the opportunity to improve business processes, especially in the parts, service and accounting departments.
				</li>
				<li>
					Built internal websites to add functionality to the ERP and scripts to automate certain tasks.
					Most notably a pure <i>Javascript</i> Workshop Scheduler that would have otherwise cost 30,000$ from an external provider.
				</li>
				<li>
					Designed and maintained the entire network topology. 3 Internet sources, 11 VLANs and 50 PCs.
					Attempted to resolve all IT issues and would escalate to our external IT support whenever necessary.
				</li>
				<li>
					Managed the implementation of a sophisticated hybrid (on/off grid) 200kw solar panel system with storage.
					Aided in improving the robustness and stability of the system by helping the technical engineer with logic and control.
				</li>
				<li>
					Supervised the expansion and renovation the new Jaguar, Bentley and Lamborghini showrooms.
					Coordinated the purchase and installation of furniture and architectural elements from foreign suppliers.
				</li>
			</ul>
		</Posting>

		<Posting position="Freelance Developer" organization="Project Chaiwala" location="Dubai, UAE" startDate="2020-10" endDate="2021-08">
			<ul>
				<li>
					Built an Extract-Load-Transform data pipeline having a FnB POS system (Revel) as source, <i>Python</i> for API access,
					<i>Postgresql</i> for storage, and <i>DBT</i> for in-database transformations. All hosted on <i>GCP</i>
				</li>
				<li>
					Created around 15 dashboards in Chartio.com for exploration and reporting purposes, served to both managers and employees.
				</li>
				<li>
					Consulted on Inventory management and internal processes to improve operational efficiencies.
				</li>
			</ul>
		</Posting>

		<Posting position="Official Match Cameraman" organization="Lebanese Rugby League" location="Lebanon" startDate="2008-01" endDate="2010-06">
			Tasked with filming all official matches, creating DVDs and uploading highlights to the website.
		</Posting>

	</div>

	<div class="flex flex-col space-y-6 m-3">

		<div class="section"><span>Projects & Achievements</span></div>

		<Posting organization="STV Lebanon" url="www.stvlebanon.com" startDate="2015-08" endDate="2020-09">
			<ul>
				<li>
					Designed a new electoral law for the parliamentary elections of Lebanon after the 2015 garbage crisis,
					realizing effective change starts from the bottom upwards.
					Wrote the algorithm using <i>Python</i> in 2015 in 3 months.
				</li>
				<li>
					Built an informative and interactive <a href="https://www.stvlebanon.com">website</a> using <i>Vue</i> and <i>Bootstrap</i> during the 2020 quarantine,
					after realizing the algorithm was to complex to explain without supporting material.
				</li>
				<li>
					Also learned 3D animation with <i>Blender</i> along with its API to create 3D simulations of elections.
				</li>
			</ul>
		</Posting>

		<Posting organization="Minteshreen" url="minteshreenelections.com" startDate="2021-12" endDate="2022-02">
			<ul>
				<li>
					Built an electoral campaign canvasing website to keep track of voter engagement and volunteer interactions.
				</li>
				<li>
					Backend uses <i>FastAPI</i> + <i>Postgresql</i> with <i>Celery</i> for background processes and <i>FastAPI-Mail</i> for volunteer registration and password management.
					Frontend uses <i>Svelte</i>, <i>Typescript</i> and <i>TailwindCSS</i>.
				</li>
			</ul>
		</Posting>

		<Posting organization="Energy Monitor" url="energy.saadtrad.com" startDate="2021-07">
			<ul>
				<li>
					Built an IOT platform, to report the energy consumption of each department.
					The information flows from power meters to an <i>ESP8266</i> microcontroller, to a <i>Python</i> service that stores the information in a <i>Postgresql</i> database.
				</li>
				<li>
					Also built a live monitoring dashboard using <i>Svelte</i>, <i>Tailwind</i> and <i>Python (Starlette)</i>.
				</li>
			</ul>
		</Posting>

		<Posting organization="Programming Contest at American University Of Beirut" startDate="2007-05">
			Placed second in the 2007 ACM programming contest where nine of the best computer science students participated.
			The top three winners would travel abroad	to compete in the regionally, then internationally.
			Unfortunately the program was canceled before the regional contest.
		</Posting>

<!--		<div class="border-2 border-teal-600 rounded text-center py-1">Other Projects can be found on <a href="https://github.com/rouppart">Github</a></div>-->

		<div class="section"><span>Education</span></div>

		<Posting position="MS In Information Technology" organization="Moscow State University" location="Moscow, Russia" startDate="2011-01" endDate="2012-07">
			<strong class="text-red-400">[Uncompleted]</strong>
			Focus on all aspects of corporate or enterprise software solutions. Courses were in Russian.
		</Posting>

		<Posting position="BS In Computer Science" organization="American University Of Beirut" location="Beirut, Lebanon" startDate="2005-09" endDate="2009-08">
				Focus on software development and included a large amount of practice from projects and lab-work. Courses were in English.
		</Posting>

		<Posting position="French Baccalaureate In Science" organization="Grand Lycee Franco Libanais" location="Beirut, Lebanon" startDate="1991" endDate="2005-06">
				Graduated with distinction in the mathematics section. Curriculum was in French.
		</Posting>

	</div>

	<div class="flex flex-col space-y-3 p-3 border-l-4">
		<div class="section"><span>Software Skills</span></div>

		<div>
			<b>Languages:</b> Python, Javascript, SQL, HTML, CSS, C++, C/AL
		</div>

		<div>
			<b>Backend Frameworks:</b> GraphQL, FastAPI, SQLAlchemy ORM, Flask
		</div>

		<div>
			<b>Frontend Frameworks:</b> Svelte, TailwindCSS, Typescript, Vue
		</div>

		<div>
			<b>Database:</b> Postgresql, Microsoft SQL Server
		</div>

		<div>
			<b>Infrastructure:</b> Docker, AWS, Google Cloud Platform
		</div>

		<div>
			<b>BI and Data Analysis:</b> Pandas, DBT, Chartio, SSRS, SSAS
		</div>

		<div>
			<b>Version Control:</b> Git
		</div>

		<div>
			<b>Operating Systems:</b> Linux Servers (Ubuntu), Linux Desktop (Manjaro, Mint), Windows Server, Windows Desktop
		</div>

		<div>
			<b>Other:</b> Microservices Architecture, Caddy Web Server, Microsoft Dynamics NAV, Arduino, ESP8266, Blender + API
		</div>

		<div class="section"><span>Other Skills</span></div>

		<div>
			<b>IT:</b> LAN, Routing, Firewall Administration, Structured Cabling, Cisco Telephony
		</div>

		<div>
			<b>Facility Management:</b> Low-Voltage Electrical Design and maintenance supervision, On/Off-Grid Solar Systems implementation,
		</div>

		<div>
			<b>Business:</b> Accounting, Inventory Management, Business Process Improvement
		</div>

		<div>
			<b>Other:</b> Welding, Brewing and Distilling Vodka
		</div>

		<div class="section"><span>Languages</span></div>

		<div class="grid" style="grid-template-columns: 1fr 2fr">
			<span>English</span><span>C2 (Fluent)</span>
			<span>French</span><span>C2 (Fluent)</span>
			<span>Arabic</span><span>C1 (Fluent)</span>
			<span>Russian</span><span>B2 (Conversational)</span>
		</div>

		<div class="section"><span>Hobbies</span></div>

		<div>
			Reading, Gym, Boxing, Wrestling, Snowboarding, Political party member.
		</div>
	</div>

</main>

<style lang="postcss">
	main {
		width: 67rem;
		display: grid;
		grid-template-columns: 1fr 1fr .8fr;
		font-family: Inter, sans-serif;
	}

	@media screen {
		main {
			@apply shadow-xl;
		}
	}

	.section {
		@apply flex justify-center;
	}

	.section span {
		@apply inline-block bg-teal-600 rounded text-white text-xl font-bold p-2 py-1 mt-2;
	}

	i {
		@apply font-bold text-gray-600;
	}
</style>
