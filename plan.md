# Project Plan: CloudHaven

**Description:** A simple web hosting platform where users can manage their domains and hosting plans.


## Development Goals

- [ ] Install Tailwind CSS using tailwindcss-rails and customize the base styling in `application.tailwind.css`.
- [ ] Implement model validations in the Domain model (models/domain.rb) to ensure name, plan and user_id are present. Validate that name is a valid domain format.
- [ ] Customize the Domain scaffold views (views/domains/*) using Tailwind CSS classes for a modern UI, focusing on index.html.erb, show.html.erb, _form.html.erb.
- [ ] Modify the Domains controller (controllers/domains_controller.rb) to associate newly created domains with the currently logged-in user using `current_user.domains.build`. Ensure that users can only manage their own domains.
- [ ] Add a 'Plans' model and scaffold, including different hosting plans (e.g., Basic, Standard, Premium) with associated storage limits and bandwidth. Allow admin users to manage plans through a separate interface.
- [ ] Create a dashboard for logged-in users (views/dashboard/index.html.erb) displaying their domains, plan usage, and account information.
- [ ] Implement basic domain status updates (e.g., Active, Suspended) and allow users to change their plan (with appropriate validation and authorization).
- [ ] Add RSpec tests for the Domain model, controller, and user authentication to ensure functionality and prevent regressions.
- [ ] Add a 'Pricing' page to display available hosting plans and their features, styled with Tailwind CSS.
- [ ] Refactor the application to improve code readability and maintainability, following Rails best practices.
