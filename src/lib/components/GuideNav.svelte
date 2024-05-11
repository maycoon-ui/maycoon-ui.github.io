<script lang="ts">
	import {
		Sidebar,
		SidebarDropdownItem,
		SidebarDropdownWrapper,
		SidebarGroup,
		SidebarItem,
		SidebarWrapper
	} from 'flowbite-svelte';
</script>

<Sidebar class="pt-20">
	<SidebarWrapper>
		<SidebarGroup>
			<SidebarDropdownWrapper label="Getting Started">
				<SidebarDropdownItem label="Installing Maycoon" />
				<SidebarDropdownItem label="Your first Project" />
				<SidebarDropdownItem label="Examples" />
			</SidebarDropdownWrapper>

			<SidebarItem label="Development Tools" />

			<SidebarDropdownWrapper label="Basic Concepts">
				<SidebarDropdownItem label="State & UI" />
				<SidebarDropdownItem label="App Control" />
				<SidebarDropdownItem label="Update Modes" />
				<SidebarDropdownItem label="Styling" />
			</SidebarDropdownWrapper>
		</SidebarGroup>

		<SidebarGroup border>
			<SidebarDropdownWrapper label="Widgets">
				<SidebarDropdownItem label="Text" />
				<SidebarDropdownItem label="Button" />
			</SidebarDropdownWrapper>
			<SidebarDropdownWrapper label="Styling">
				<SidebarDropdownItem label="Themes" />
				<SidebarDropdownItem label="Schemes" />
			</SidebarDropdownWrapper>
		</SidebarGroup>

		<SidebarGroup border>
			<SidebarDropdownWrapper label="Testing & Debugging">
				<SidebarDropdownItem label="Tests" />
				<SidebarDropdownItem label="Debugging Tools" />
			</SidebarDropdownWrapper>
		</SidebarGroup>

		<SidebarGroup border>
			<SidebarDropdownWrapper label="Code & App Style">
				<SidebarDropdownItem label="Linting" />
				<SidebarDropdownItem label="DOs & DON'Ts" />
			</SidebarDropdownWrapper>
		</SidebarGroup>

		<SidebarGroup border>
			<SidebarDropdownWrapper label="Deployment">
				<SidebarDropdownItem label="Building for Release" />
				<SidebarDropdownItem label="Publishing your App" />
				<SidebarDropdownItem label="Licensing" />
			</SidebarDropdownWrapper>
		</SidebarGroup>

		<SidebarGroup border>
			<SidebarDropdownWrapper label="Tuning Maycoon">
				<SidebarDropdownItem label="Settings" />
				<SidebarDropdownItem label="Higher Performance" />
				<SidebarDropdownItem label="Shorter Compile Times" />
				<SidebarDropdownItem label="App Size" />
			</SidebarDropdownWrapper>

			<SidebarDropdownWrapper label="Expanding Maycoon">
				<SidebarDropdownItem label="Creating Plugins" />
				<SidebarDropdownItem label="Making custom Widgets" />
				<SidebarDropdownItem label="Custom Styles & Themes" />
			</SidebarDropdownWrapper>
		</SidebarGroup>

		<SidebarGroup border>
			<SidebarItem label="Github Actions" />
		</SidebarGroup>

		<SidebarGroup border>
			<SidebarItem label="Contribution Quick Starter" />
			<SidebarDropdownWrapper label="Contributing">
				<SidebarDropdownItem label="Code has Rules" />
				<SidebarDropdownItem label="Crates & Components" />
				<SidebarDropdownItem label="Tools & Dependencies" />
				<SidebarDropdownItem label="Core Render Concepts" />
			</SidebarDropdownWrapper>
		</SidebarGroup>
	</SidebarWrapper>
</Sidebar>
