# SNHU-Software-Test-Automation-QA

# How can I ensure that my code, program, or software is functional and secure?
To ensure functionality, I apply rigorous testing strategies, including unit tests, integration tests, and boundary testing. For instance, in the Contact and ContactService classes, I created test cases that validate the input constraints, check for edge cases (e.g., invalid phone numbers or overly long fields), and confirm expected behavior under normal conditions.

Security is addressed by validating all user inputs and preventing malicious or invalid data from being processed. For example, the constructors and setter methods in the Contact class enforce strict length and format constraints, rejecting inputs that do not meet the criteria. This minimizes vulnerabilities, such as injection attacks or buffer overflows. Additionally, by handling null values and maintaining a secure storage mechanism (e.g., HashMap for in-memory data), the software is designed to be robust and secure.

# How do I interpret user needs and incorporate them into a program?
Understanding user needs begins with clear and detailed requirements. For this project, the requirements specified that each contact should have unique attributes (e.g., ID, first name, phone number) and that these attributes should adhere to strict validation rules. By implementing constructors and setter methods that enforce these rules, I ensured that the program would only accept valid data, aligning with user expectations for reliability.

Additionally, flexibility was incorporated by allowing updates to specific attributes without altering the rest of the contact data. For example, in the ContactService class, the updateContact method enables partial updates while maintaining existing validated data. This approach reflects an understanding of real-world use cases where users may need to modify certain fields while preserving others.

# How do I approach designing software?
My design process emphasizes modularity, clarity, and adherence to requirements. For instance, I divided the project into three main components: the Contact class (defining individual contacts), the ContactService class (managing a collection of contacts), and comprehensive test classes (ContactTest and ContactServiceTest). This separation of concerns ensures that each component is focused and testable, which simplifies maintenance and future enhancements.

I follow object-oriented principles, such as encapsulation and validation. All fields in the Contact class are private, with controlled access through getters and setters. This design ensures data integrity and shields internal implementation details from external manipulation.

Finally, testing is integral to the design process. By writing tests concurrently with the implementation, I could identify and address issues early, ensuring that the software meets its functional and performance goals.

