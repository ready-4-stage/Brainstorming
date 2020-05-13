# Brainstorming

This repository intends as an area where we can collect ideas until we begin with the development phase. Will be deleted once we start coding.

## Technologies

Technology | Proposal
------------ | -------------
Programming language | Java 11 (OpenJDK)
Database | SQLite
UI | Swing
Validation | `javax.validation`
Other | Lombok, Log4J (SLF4J)

## Structure

### Multi-Module-Project (Maven)
- `database`: contains the DAOs (via an interface)
- `model`: our models (as Java POJO's with Lombok); used in all modules
- `server`: a REST-Service (SpringBoot) providing the link between the `database` and `UI`
- `ui`: a UI in Swing; connects to the `server`
