# CA
CA is a phone application for weigh cocoa and copra.import androidx.room.Database
import androidx.room.RoomDatabase

@Database(entities = [WeightRecord::class], version = 1)
abstract class AppDatabase : RoomDatabase() {
    abstract fun weightRecordDao(): WeightRecordDao
}
