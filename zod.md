https://zod.dev/

// ezzel lehet ellenőrizni, hogy a beérkező adat megfelel-e a kívánt strukturának

npm install zod

import { z } from "zod"

export const PersonSchema = z.object({
    name: z.string(),
    data: z.object({
        age: z.number(),
        gender: z.literal("male").or(z.literal("female"))
    })
})

import {PersonSchema} from "./helye"

const isValidData = PersonSchema.parse(jsonData)
type Person = z.infer<typeof PersonSchema>