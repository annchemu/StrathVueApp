<template>
    <div id = 'homepage'>
        <v-container>
                <v-layout column>
                    <v-carousel>
                        <v-carousel-item
                            src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                            cover
                        ></v-carousel-item>
                    </v-carousel>
                    </v-layout>
                    <v-layout>
                    <v-container>
                        <v-row align="center" justify="center">
                            <div class="d-flex align-center flex-column">

                                <v-card width="400">
                                <v-card-item>
                                    <v-card-title>{{ componentTitle }}</v-card-title>
                                </v-card-item>

                                <v-card-text>
                                    <v-table>
                                        <thead>
                                        <tr>
                                            <th class="text-left">
                                            Name
                                            </th>
                                           
                                        </tr>
                                        </thead>
                                        <tbody>
                                        <tr
                                            v-for="course in courses"
                                            :key="course.id"
                                        >
                                            <td>
                                                <v-btn to="/newcomponent" color="primary">{{ course.coursename }}</v-btn>
                                            </td>
                                        </tr>
                                        </tbody>
                                    </v-table>
                                </v-card-text>
                                </v-card>
                            </div>
                        </v-row>
                    </v-container>
                </v-layout>
            </v-container>
    </div>
</template>
<script>
export default {
  data() {
    return {
      courses:[
        {
            id: 1,
            coursename: 'Financial Economics'
        },
        {
            id: 2,
            course_name: 'Computer Science'
        },
        {
            id: 3,
            coursename: 'Computer Science'
        },
        {
            id: 4,
            coursename: 'Financial Engineering'
        },
        {
            id: 5,
            coursename: 'Medicine and Surgery'
        },
        {
            id: 6,
            coursename: 'Education'
        },
        {
            id: 7,
            coursename: 'Architecture'
        },
        {
            id: 8,
            coursename: 'Forestry'
        },
        {
            id: 9,
            coursename: 'Law'
        },
        {
            id: 10,
            coursename: ' Hospitality and Tourism'
        }
      ],
      componentTitle: 'Courses at Strath Uni'
    }
  },
  methods: {
    addCoursesLocation() {
      for(course in courses){			//courses is an array containing all the courses in the app
	course.location = 'Nairobi'		// adding a new element to the array
    }
  }
  },
  mounted() {
    console.log(this.courses)
  }
}
</script>

