## How do Pick and Omit utility types prevent code duplication while creating specialized "slices" of a master interface? Discuss how this keeps your code DRY (Don't Repeat Yourself).

Pick and Omit are utility types used to create smaller versions of an existing interface, helping us follow the DRY (Don't Repeat Yourself) principle.
Pick:

Pick selects specific properties from an interface.

interface User {
  id: number;
  name: string;
  email: string;
}
type UserPreview = Pick<User, "name" | "email">;


Omit:
Omit removes specific properties from an interface.
type UserWithoutEmail = Omit<User, "email">;