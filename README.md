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

- `common`: common classes such as our models (as Java POJO's with Lombok); used in all modules
- `database`: contains the DAOs (via an interface); may be implemented as Spring-Beans
- `server`: a REST-Service (SpringBoot) providing the link between the `database` and `ui` by using `common`
- `ui`: a UI in Swing; connects to the `server`

#### Possible file structure:

- `stage-common/`
- `stage-database/`
- `stage-server/`
- `stage-ui/`
- `pom.ml`

## Other

- Authentication via Bearer Token (OAuth)
