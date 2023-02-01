<script lang="ts">
  import {
    Collapse,
    Navbar,
    NavbarToggler,
    NavbarBrand,
    Nav,
    NavItem,
    NavLink,
  } from "sveltestrap";

  let isOpen = false;
  const toggle = () => (isOpen = !isOpen);
</script>

<Navbar color="dark" dark>
  <NavbarBrand href="/" class="me-auto">topic</NavbarBrand>
  <NavbarToggler on:click={toggle} class="me-2" />
  <Collapse {isOpen} navbar>
    <Nav navbar>
      <NavItem>
        <NavLink href="/">Home</NavLink>
      </NavItem>
    </Nav>
  </Collapse>
</Navbar>
